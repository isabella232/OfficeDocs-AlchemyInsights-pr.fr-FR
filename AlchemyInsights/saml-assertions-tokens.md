---
title: Assertions SAML (jetons)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884588"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="512e7-102">Assertions SAML (jetons)</span><span class="sxs-lookup"><span data-stu-id="512e7-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="512e7-103">Les jetons SAML (Security Assertions Markup Language) sont des représentations XML des revendications.</span><span class="sxs-lookup"><span data-stu-id="512e7-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="512e7-104">Par défaut, les jetons SAML que Windows Communication Foundation (WCF) utilise dans les scénarios de sécurité fédérée sont des jetons émis.</span><span class="sxs-lookup"><span data-stu-id="512e7-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="512e7-105">Pour plus d’informations, [voir Jetons SAML et revendications.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="512e7-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="512e7-106">La plateforme d’identités Microsoft émet plusieurs types de jetons de sécurité dans le traitement de chaque flux d’authentification.</span><span class="sxs-lookup"><span data-stu-id="512e7-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="512e7-107">[La référence des revendications de](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) jeton SAML décrit le format, les caractéristiques de sécurité et le contenu des jetons SAML 2.0.</span><span class="sxs-lookup"><span data-stu-id="512e7-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="512e7-108">Suivez les instructions de la plateforme d’identités Microsoft sur les durées de vie des jetons [configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) pour comprendre comment configurer les durées de vie des jetons.</span><span class="sxs-lookup"><span data-stu-id="512e7-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="512e7-109">Suivez les étapes décrites dans [cet article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) pour comprendre comment configurer le chiffrement de jeton SAML Azure AD.</span><span class="sxs-lookup"><span data-stu-id="512e7-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="512e7-110">Dans Azure AD, vous pouvez configurer les options de signature de certificat et l’algorithme de signature de certificat.</span><span class="sxs-lookup"><span data-stu-id="512e7-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="512e7-111">Pour plus d’informations, voir options avancées de signature de certificat dans le jeton SAML pour les applications de galerie [dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="512e7-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
