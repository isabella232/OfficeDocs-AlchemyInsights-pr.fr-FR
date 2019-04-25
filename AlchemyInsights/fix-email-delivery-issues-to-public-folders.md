---
title: Corriger les problèmes de remise des messages électroniques dans les dossiers publics à extension messagerie
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401326"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="4d0db-102">Corriger les problèmes de remise des messages électroniques dans les dossiers publics à extension messagerie</span><span class="sxs-lookup"><span data-stu-id="4d0db-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="4d0db-103">Si les expéditeurs externes ne peuvent pas envoyer de messages à vos dossiers publics à extension messagerie et que les expéditeurs reçoivent l'erreur suivante: introuvable **(550 5.4.1)**, vérifiez que le domaine de messagerie du dossier public est configuré en tant que domaine de relais interne au lieu d'un domaine faisant autorité:</span><span class="sxs-lookup"><span data-stu-id="4d0db-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="4d0db-104">Ouvrez le [Centre d'administration Exchange](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4d0db-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="4d0db-105">Accédez à \*\*\*\* \> **domaines**de flux de messagerie acceptés, sélectionnez le domaine accepté, puis cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="4d0db-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="4d0db-106">Dans la page des propriétés qui s'ouvre, si le type de domaine est défini sur **authoritative**, modifiez la valeur sur **relais interne** , puis cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="4d0db-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="4d0db-107">Si les expéditeurs externes reçoivent l'erreur « **vous n'avez pas l'autorisation (550 5.7.13)**, exécutez la commande suivante dans [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pour voir les autorisations pour les utilisateurs anonymes dans le dossier public:</span><span class="sxs-lookup"><span data-stu-id="4d0db-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="4d0db-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Par exemple, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="4d0db-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="4d0db-109">Pour autoriser les utilisateurs externes à envoyer des messages électroniques à ce dossier public, ajoutez le droit d'accès CreateItems à l'utilisateur anonyme.</span><span class="sxs-lookup"><span data-stu-id="4d0db-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="4d0db-110">Par exemple, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="4d0db-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
