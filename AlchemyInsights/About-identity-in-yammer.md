---
title: À propos de l’identité dans Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146776"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="fee06-102">À propos de l’identité dans Yammer</span><span class="sxs-lookup"><span data-stu-id="fee06-102">About identity in Yammer</span></span>

<span data-ttu-id="fee06-103">Nous vous recommandons de suivre les étapes suivantes pour tous les réseaux dans le but d’éviter les problèmes liés à l’identité :</span><span class="sxs-lookup"><span data-stu-id="fee06-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="fee06-104">Appliquez l’identité Office 365 après la mise en service des comptes Microsoft 365 pour les utilisateurs dans Azure Active Directory pour vérifier que tous les utilisateurs se connectent à l’aide de leur compte Microsoft 365 principal.</span><span class="sxs-lookup"><span data-stu-id="fee06-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="fee06-105">Pour obtenir davantage d’informations, voir [Appliquer l’identité Office 365 pour les utilisateurs Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="fee06-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="fee06-106">Consolidez plusieurs réseaux Yammer.</span><span class="sxs-lookup"><span data-stu-id="fee06-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="fee06-107">Les configurations Yammer héritées autorisent la connexion de plusieurs réseaux Yammer à un client.</span><span class="sxs-lookup"><span data-stu-id="fee06-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="fee06-108">Pour obtenir davantage d'informations, consultez l'article [Migration réseau : consolider plusieurs réseaux Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="fee06-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="fee06-109">Vous pouvez également appliquer les licences pour Yammer afin de bloquer les utilisateurs de Yammer qui ne disposent pas de licence.</span><span class="sxs-lookup"><span data-stu-id="fee06-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="fee06-110">Si vous souhaitez en savoir plus, consultez [Gérer les licences utilisateur de Yammer dans Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="fee06-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="fee06-111">Enfin, auditez la liste des utilisateurs pour les anciens réseaux Yammer et suspendez les utilisateurs hérités.</span><span class="sxs-lookup"><span data-stu-id="fee06-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="fee06-112">Il est recommandé de suspendre (désactiver) les utilisateurs au lieu de les supprimer, car leur suppression est irréversible.</span><span class="sxs-lookup"><span data-stu-id="fee06-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="fee06-113">Pour obtenir davantage d’informations, voir [Audit des utilisateurs de Yammer dans des réseaux connectés à Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) et [Supprimer des utilisateurs](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="fee06-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="fee06-114">En configurant Yammer à l’aide de ces étapes, vous serez également prêt à configurer votre réseau Yammer en mode natif pour Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fee06-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="fee06-115">Pour obtenir davantage d’informations, consultez [Configurer votre réseau Yammer en mode natif pour Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="fee06-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>