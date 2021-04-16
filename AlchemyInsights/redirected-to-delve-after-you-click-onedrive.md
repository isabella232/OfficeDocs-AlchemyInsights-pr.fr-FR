---
title: OneDrive Entreprise Web OneDrive redirige vers Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799987"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="984e7-102">Redirigé vers Delve après avoir cliqué sur OneDrive</span><span class="sxs-lookup"><span data-stu-id="984e7-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="984e7-103">Consultez notre guide [de dépannage détaillé.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="984e7-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="984e7-104">Pour résoudre ce problème, l'administrateur doit accorder aux utilisateurs le droit de créer leur site Mes sites.</span><span class="sxs-lookup"><span data-stu-id="984e7-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="984e7-105">Cela est dû au fait que la page OneDrive Entreprise est créée sur Mes sites.</span><span class="sxs-lookup"><span data-stu-id="984e7-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="984e7-106">Pour accorder ce droit, suivez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="984e7-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="984e7-107">Dans le Centre d'administration SharePoint, cliquez sur **profils utilisateur.**</span><span class="sxs-lookup"><span data-stu-id="984e7-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="984e7-108">Dans la section **Personnes,** cliquez sur **Gérer les autorisations utilisateur.**</span><span class="sxs-lookup"><span data-stu-id="984e7-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="984e7-109">Ajoutez les utilisateurs qui ont besoin d'autorisations pour créer leur site Mes sites.</span><span class="sxs-lookup"><span data-stu-id="984e7-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="984e7-110">Par défaut, ce paramètre est définie sur Tout le monde **sauf les utilisateurs externes.**</span><span class="sxs-lookup"><span data-stu-id="984e7-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="984e7-111">Une fois que vous avez ajouté l'utilisateur, les utilisateurs ou le groupe, assurez-vous que l'utilisateur, les utilisateurs ou le groupe ajoutés est sélectionné, faites défiler la section **autorisations,** puis cochez la case en regard de Créer un site personnel (requis pour le stockage personnel, le **newsfeed** et le contenu suivi).</span><span class="sxs-lookup"><span data-stu-id="984e7-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="984e7-112">Cliquez **sur OK,** puis faites en cas d'accès de l'utilisateur à la page OneDrive pour créer le site.</span><span class="sxs-lookup"><span data-stu-id="984e7-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
