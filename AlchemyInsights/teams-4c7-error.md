---
title: Erreur Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786667"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="d8579-102">Erreur 4c7 dans Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d8579-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="d8579-103">Cette erreur se produit car Microsoft Teams requiert l'authentification par formulaires.</span><span class="sxs-lookup"><span data-stu-id="d8579-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="d8579-104">Lorsque vous déployez les services AD FS (Active Directory Federation Services), l'authentification par formulaires n'est pas activée pour l'intranet par défaut.</span><span class="sxs-lookup"><span data-stu-id="d8579-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="d8579-105">Si l'authentification intégrée Windows échoue, vous êtes invité à vous inscrire à l'aide de l'authentification par formulaires.</span><span class="sxs-lookup"><span data-stu-id="d8579-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="d8579-106">Pour résoudre ce problème, activez l'authentification par formulaires à l'aide du logiciel en snap-in MMC (Microsoft Management Console) AD FS sur l'ordinateur qui dispose de la copie locale d'Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8579-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="d8579-107">Pour cela, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="d8579-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="d8579-108">Dans le volet de navigation, accédez aux stratégies **d'authentification.**</span><span class="sxs-lookup"><span data-stu-id="d8579-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="d8579-109">Sous **Actions dans** le volet d'informations, **sélectionnez Modifier l'authentification principale globale.**</span><span class="sxs-lookup"><span data-stu-id="d8579-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="d8579-110">Sous **l'onglet Intranet,** sélectionnez **Authentification par formulaires.**</span><span class="sxs-lookup"><span data-stu-id="d8579-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="d8579-111">Sélectionnez **OK** (ou **Appliquer).**</span><span class="sxs-lookup"><span data-stu-id="d8579-111">Select **OK** (or **Apply**).</span></span>