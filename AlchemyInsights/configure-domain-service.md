---
title: Configurer le service de domaine
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
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="b6f32-102">Échec de l’installation d’AAD-DS ou du déploiement</span><span class="sxs-lookup"><span data-stu-id="b6f32-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="b6f32-103">Pour résoudre le problème d’échec d’activation ou de déploiement du service de domaine Azure AD (AAD-DS), effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="b6f32-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="b6f32-104">Si vous utilisez un réseau virtuel existant, recherchez dans votre NSG des règles qui bloquent les ports nécessaires à la synchronisation dans AAD-DS dans le portail https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="b6f32-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="b6f32-105">Vérifiez si le message d’erreur que vous avez reçu est traité dans ce guide de dépannage disponible dans  https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="b6f32-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="b6f32-106">Essayez de déployer les services de domaine Azure AD dans un nouveau réseau virtuel.</span><span class="sxs-lookup"><span data-stu-id="b6f32-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="b6f32-107">Suivez le guide de mise en service pour déployer AAD-DS : [Créer et configurer des services de domaine AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="b6f32-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="b6f32-108">Si vous n’arrivez pas à déployer les services de domaine Azure AD, voir [Résoudre les problèmes d'Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pour résoudre les erreurs courantes afin de résoudre les problèmes.</span><span class="sxs-lookup"><span data-stu-id="b6f32-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="b6f32-109">**Impossible de désactiver AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="b6f32-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="b6f32-110">AAD-DS ne peut pas être mis en pause.</span><span class="sxs-lookup"><span data-stu-id="b6f32-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="b6f32-111">Si vous souhaitez arrêter d’utiliser votre domaine géré, il doit être supprimé.</span><span class="sxs-lookup"><span data-stu-id="b6f32-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="b6f32-112">Pour supprimer votre domaine géré, voir supprimer [Service de domaine AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="b6f32-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



