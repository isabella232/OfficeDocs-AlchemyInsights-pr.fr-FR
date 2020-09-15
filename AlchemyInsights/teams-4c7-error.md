---
title: Erreur 4C7 teams
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700201"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="16c95-102">erreur 4C7 dans Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="16c95-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="16c95-103">Cette erreur se produit parce que Microsoft teams nécessite l’authentification par formulaire.</span><span class="sxs-lookup"><span data-stu-id="16c95-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="16c95-104">Lorsque vous déployez Active Directory Federation Services (AD FS), l’authentification par formulaire n’est pas activée par défaut pour l’intranet.</span><span class="sxs-lookup"><span data-stu-id="16c95-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="16c95-105">Si l’authentification Windows intégrée échoue, vous êtes invité à vous connecter à l’aide de l’authentification par formulaire.</span><span class="sxs-lookup"><span data-stu-id="16c95-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="16c95-106">Pour résoudre ce problème, activez l’authentification par formulaire à l’aide du composant logiciel enfichable MMC (Microsoft Management Console) AD FS sur l’ordinateur disposant de la copie locale d’Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16c95-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="16c95-107">Pour cela, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="16c95-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="16c95-108">Dans le volet de navigation, accédez à **stratégies d’authentification**.</span><span class="sxs-lookup"><span data-stu-id="16c95-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="16c95-109">Sous **actions** dans le volet d’informations, sélectionnez **modifier l’authentification principale globale**.</span><span class="sxs-lookup"><span data-stu-id="16c95-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="16c95-110">Sous l’onglet **Intranet** , sélectionnez **authentification par formulaire**.</span><span class="sxs-lookup"><span data-stu-id="16c95-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="16c95-111">Sélectionnez **OK** (ou **appliquer**).</span><span class="sxs-lookup"><span data-stu-id="16c95-111">Select **OK** (or **Apply**).</span></span>