---
title: Résolution des applications Microsoft 365 les licences Office n’ont pas pu être détectées message associé
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747693"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="ed5cf-102">Résolution du message « Impossible de trouver des licences Office associées » pour Microsoft 365 apps</span><span class="sxs-lookup"><span data-stu-id="ed5cf-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="ed5cf-103">Si vous recevez ce message, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ed5cf-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ed5cf-104">Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ed5cf-105">Voir [URL et plages d’adresses IP Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ed5cf-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="ed5cf-106">Supprimez et [réaffectez la licence Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pour l’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="ed5cf-107">Ouvrez une application Office et [déconnectez-vous](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de tous les comptes d’utilisateurs existants.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="ed5cf-108">Accédez à paramètres **Windows > comptes**de & de  >  **messagerie**et supprimez tous les comptes de travail sauf le compte affecté.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="ed5cf-109">Accédez à paramètres Windows > **comptes**  >  **accès professionnel ou scolaire**, puis déconnectez tous les comptes professionnels à l’exception du compte affecté.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="ed5cf-110">Réinitialisez l’état d’activation d’Office.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-110">Reset the Office activation state.</span></span> <span data-ttu-id="ed5cf-111">[Découvrir comment](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="ed5cf-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="ed5cf-112">[Connectez-vous](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) à l’aide du compte d’utilisateur affecté.</span><span class="sxs-lookup"><span data-stu-id="ed5cf-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="ed5cf-113">Pour obtenir des solutions de résolution des problèmes supplémentaires, consultez la rubrique [Erreurs d’activation et de produit sans licence dans Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="ed5cf-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>