---
title: 'Contrôleur de domaine '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886847"
---
# <a name="domain-controller"></a><span data-ttu-id="73571-102">Contrôleur de domaine</span><span class="sxs-lookup"><span data-stu-id="73571-102">Domain controller</span></span>

<span data-ttu-id="73571-103">**Échec de l’installation d’AAD-DS ou du déploiement**</span><span class="sxs-lookup"><span data-stu-id="73571-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="73571-104">Pour résoudre le problème d’échec d’activation ou de déploiement du service de domaine Azure AD (AAD-DS), effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="73571-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="73571-105">Si vous utilisez un réseau virtuel existant, recherchez dans votre NSG des règles qui bloquent les ports nécessaires à la synchronisation dans AAD-DS dans le portail https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="73571-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="73571-106">Vérifiez si le message d’erreur que vous avez reçu est traité dans ce guide de dépannage disponible dans  https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="73571-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="73571-107">Essayez de déployer les services de domaine Azure AD dans un nouveau réseau virtuel.</span><span class="sxs-lookup"><span data-stu-id="73571-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="73571-108">Suivez le guide de mise en service pour déployer AAD-DS : [Tutoriel pour créer des services de domaine AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="73571-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="73571-109">Si vous n’arrivez pas à déployer les services de domaine Azure AD, voir [Résoudre les problèmes d'Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pour résoudre les erreurs courantes afin de résoudre les problèmes.</span><span class="sxs-lookup"><span data-stu-id="73571-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="73571-110">**Impossible de désactiver AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="73571-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="73571-111">AAD-DS ne peut pas être mis en pause.</span><span class="sxs-lookup"><span data-stu-id="73571-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="73571-112">Si vous souhaitez arrêter d’utiliser votre domaine géré, il doit être supprimé.</span><span class="sxs-lookup"><span data-stu-id="73571-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="73571-113">Si vous rencontrez un problème, pour résoudre les messages d’erreur courants et pour consulter les étapes de dépannage qui vous aideront à reprendre votre travail, voir [Résolution des problèmes liés aux services de domaine Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="73571-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
