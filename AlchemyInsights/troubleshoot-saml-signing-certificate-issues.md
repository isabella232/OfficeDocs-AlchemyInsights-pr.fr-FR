---
title: Résoudre des problèmes de certificat de signature SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529210"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="f6cc9-102">Résoudre les problèmes de certificat de signature SAML</span><span class="sxs-lookup"><span data-stu-id="f6cc9-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="f6cc9-103">Pour résoudre un problème de certificat de signature SAML, ces étapes recommandées :</span><span class="sxs-lookup"><span data-stu-id="f6cc9-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="f6cc9-104">Lorsque vous ajoutez une application d’entreprise qui prend en charge l’authentification unique, Azure génère un certificat appelé [Certificat de signature SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="f6cc9-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="f6cc9-105">Ce certificat a une date d’expiration de 3 ans.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="f6cc9-106">Pour modifier la date d’expiration de votre certificat, consultez [Personnaliser la date d’expiration de votre certificat de fédération et en faire un nouveau certificat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="f6cc9-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="f6cc9-107">Azure utilisera ce certificat pour signer les jetons SAML demandés par l’application et les envoyer à l’application pour que l’authentification unique s’effectue.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="f6cc9-108">Pour ce faire, téléchargez le certificat à partir du portail Azure et envoyez-le au fournisseur de l’application pour finalisation du processus d’authentification unique.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="f6cc9-109">Une fois ce processus terminé, votre application prendra en compte ce certificat et tous les jetons SAML signés par ce certificat seront acceptés par l’application.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="f6cc9-110">Si ce certificat arrive à expiration, créez-en un, informez le fournisseur de l’application, puis activez-le sur Azure.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="f6cc9-111">Pour plus d’informations, consultez [Renouveler un certificat expirant bientôt](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="f6cc9-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="f6cc9-112">Si le certificat expire, l’utilisateur n’est pas bloqué.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="f6cc9-113">[Ajoutez une adresse pour les notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) avant l’expiration du certificat actuel.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="f6cc9-114">L’étape 4 est facultative.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="f6cc9-115">Modifiez les options de signature du certificat SAML d’une application ainsi que l’algorithme de signature du certificat.</span><span class="sxs-lookup"><span data-stu-id="f6cc9-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="f6cc9-116">Pour plus d’informations, consultez [Modifier des options de signature de certificat et d’un algorithme de signature](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="f6cc9-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

