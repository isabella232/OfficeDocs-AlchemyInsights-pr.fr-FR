---
title: Configurer Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884593"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="88e92-102">Échec de l’activation d’AAD-DS ou du déploiement</span><span class="sxs-lookup"><span data-stu-id="88e92-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="88e92-103">Pour résoudre le problème d’échec d’activation ou de déploiement de Azure Active Directory Domain Services (AAD-DS), procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="88e92-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="88e92-104">Si vous utilisez un réseau virtuel existant, vérifiez les règles NSG qui bloquent les ports nécessaires à la synchronisation dans AAD-DS dans le portail https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="88e92-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="88e92-105">Vérifiez si le message d’erreur que vous avez reçu est traité dans ce guide de dépannage disponible sur la page https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="88e92-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="88e92-106">Essayez de déployer AAD-DS dans un nouveau réseau virtuel.</span><span class="sxs-lookup"><span data-stu-id="88e92-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="88e92-107">Suivez le guide de prise en main pour apprendre à déployer AAD-DS : [Créer et configurer un domaine managé Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="88e92-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="88e92-108">Si vous n’arrivez pas à déployer AAD-DS, veuillez consulter la page [Erreurs courantes et étapes de dépannage pour Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pour découvrir quelles sont les erreurs courantes et trouver comment les résoudre.</span><span class="sxs-lookup"><span data-stu-id="88e92-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="88e92-109">**Impossible de désactiver AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="88e92-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="88e92-110">AAD-DS ne peut pas être mis en pause.</span><span class="sxs-lookup"><span data-stu-id="88e92-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="88e92-111">Si vous souhaitez arrêter d’utiliser votre domaine géré, il doit être supprimé.</span><span class="sxs-lookup"><span data-stu-id="88e92-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="88e92-112">Pour supprimer votre domaine géré, veuillez consulter la page [Désactiver ou supprimer un domaine managé Azure Active Directory Domain Services à partir du portail Azure](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="88e92-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



