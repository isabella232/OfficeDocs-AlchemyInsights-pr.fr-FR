---
title: Le certificat Push Apple GPM n’a pas été configuré
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431461"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="0212f-102">Le certificat Push Apple GPM n’a pas été configuré</span><span class="sxs-lookup"><span data-stu-id="0212f-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="0212f-103">Un certificat Push Apple GPM (également appelé certificat Push Apple Notification Service (APNS)) n’a pas été configuré pour votre abonnement.</span><span class="sxs-lookup"><span data-stu-id="0212f-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="0212f-104">Si vous n’avez pas configuré un certificat Apple GPM push, vous ne pouvez pas inscrire et gérer les appareils iOS et MacOS.</span><span class="sxs-lookup"><span data-stu-id="0212f-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="0212f-105">Après avoir ajouté le certificat à Intune, les utilisateurs peuvent installer l'application Company Portal pour enregistrer leurs appareils iOS.</span><span class="sxs-lookup"><span data-stu-id="0212f-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="0212f-106">Sélectionnez **« J’accepte ».**</span><span class="sxs-lookup"><span data-stu-id="0212f-106">Select **"I agree."**</span></span> <span data-ttu-id="0212f-107">pour accorder à Microsoft l’autorisation d’envoyer des données à Apple.</span><span class="sxs-lookup"><span data-stu-id="0212f-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="0212f-108">Sélectionnez **Télécharger votre conseiller du service clientèle** la demande de signature de certificat Intune requise pour créer un certificat Apple GPM pour Push.</span><span class="sxs-lookup"><span data-stu-id="0212f-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="0212f-109">Le fichier est utilisé pour demander un certificat de relation de confiance à partir du Portail de certificats Push Apple.</span><span class="sxs-lookup"><span data-stu-id="0212f-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="0212f-110">Sélectionnez **Créer votre certificat Push GPM** pour accéder au Portail certificats Push Apple.</span><span class="sxs-lookup"><span data-stu-id="0212f-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="0212f-111">Connectez-vous avec l'identifiant Apple de votre entreprise, puis sélectionnez **Créer un certificat**.</span><span class="sxs-lookup"><span data-stu-id="0212f-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="0212f-112">Sélectionnez **Choisir fichier**, accédez au fichier de demande de signature de certificat, puis sélectionnez **Télécharger**.</span><span class="sxs-lookup"><span data-stu-id="0212f-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="0212f-113">Sur la page de confirmation, sélectionnez **Télécharger** pour télécharger le fichier (.pem) du certificat et enregistrer le fichier en local.</span><span class="sxs-lookup"><span data-stu-id="0212f-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="0212f-114">**Remarque**: le certificat est associé à l’ID Apple utilisé pour le créer.</span><span class="sxs-lookup"><span data-stu-id="0212f-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="0212f-115">Nous vous conseillons d’utiliser un ID Apple d’entreprise pour les tâches de gestion et de vérifier que la boîte aux lettres est contrôlée par plusieurs personnes ou à l’aide d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0212f-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="0212f-116">N'utilisez jamais un identifiant Apple personnel.</span><span class="sxs-lookup"><span data-stu-id="0212f-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="0212f-117">Utilisez le même ID Apple pour renouveler le certificat Push Apple tous les 12 mois.</span><span class="sxs-lookup"><span data-stu-id="0212f-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="0212f-118">Entrez l'ID Apple utilisé pour créer votre certificat de push GPM Apple.</span><span class="sxs-lookup"><span data-stu-id="0212f-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="0212f-119">Enregistrez cet ID comme rappel pour lorsque vous avez besoin de renouveler le certificat.</span><span class="sxs-lookup"><span data-stu-id="0212f-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="0212f-120">Accédez au fichier de certificat (.pem), sélectionnez **Ouvrir**, puis sélectionnez **Télécharger**.</span><span class="sxs-lookup"><span data-stu-id="0212f-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="0212f-121">Avec le certificat push, Intune peut inscrire et gérer les appareils Apple.</span><span class="sxs-lookup"><span data-stu-id="0212f-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>