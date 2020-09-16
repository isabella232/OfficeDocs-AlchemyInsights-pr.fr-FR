---
title: Onedrive entreprise Web OneDrive redirige vers Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776377"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="144ea-102">Redirigé vers Delve après avoir cliqué sur OneDrive</span><span class="sxs-lookup"><span data-stu-id="144ea-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="144ea-103">Consultez notre [Guide de dépannage](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)détaillé.</span><span class="sxs-lookup"><span data-stu-id="144ea-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="144ea-104">Pour résoudre ce problème, l’administrateur doit accorder aux utilisateurs le droit de créer leur site mes sites.</span><span class="sxs-lookup"><span data-stu-id="144ea-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="144ea-105">Cela est dû au fait que la page OneDrive entreprise est créée sur les sites mon site.</span><span class="sxs-lookup"><span data-stu-id="144ea-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="144ea-106">Pour accorder ce droit, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="144ea-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="144ea-107">Dans le centre d’administration SharePoint, cliquez sur **profils utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="144ea-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="144ea-108">Dans la section **personnes** , cliquez sur **gérer les autorisations des utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="144ea-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="144ea-109">Ajoutez des utilisateurs qui requièrent des autorisations pour créer leur site mes sites.</span><span class="sxs-lookup"><span data-stu-id="144ea-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="144ea-110">Par défaut, ce paramètre est défini sur **tout le monde sauf les utilisateurs externes**.</span><span class="sxs-lookup"><span data-stu-id="144ea-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="144ea-111">Une fois que vous avez ajouté l’utilisateur, les utilisateurs ou le groupe, vérifiez que l’utilisateur, les utilisateurs ou le groupe ajouté est sélectionné, faites défiler jusqu’à la section **autorisations** , puis activez la case à cocher en regard de **créer un site personnel (requis pour le stockage personnel, le flux d’actualités et le contenu suivi)**.</span><span class="sxs-lookup"><span data-stu-id="144ea-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="144ea-112">Cliquez sur **OK**, puis demandez à l’utilisateur d’accéder à la page OneDrive pour créer le site.</span><span class="sxs-lookup"><span data-stu-id="144ea-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
