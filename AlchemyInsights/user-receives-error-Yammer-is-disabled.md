---
title: L’utilisateur reçoit l’erreur AADSTS7000112 Yammer est désactivé
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157298"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="8d2c2-102">L’utilisateur reçoit l’erreur AADSTS7000112 Yammer est désactivé</span><span class="sxs-lookup"><span data-stu-id="8d2c2-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="8d2c2-103">Si le message d’erreur « AADSTS7000112 : L’application '00000005-0000-0ff1-CE00-000000000000'(Yammer) est désactivée » s’affiche, cela indique qu’il existe un problème avec le principal de service dans Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="8d2c2-104">Un administrateur a peut-être désactivé le principal de service pour bloquer l’accès à Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="8d2c2-105">La désactivation du principal de service n’est pas recommandée et peut entraîner d’autres problèmes.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="8d2c2-106">Pour plus d’informations sur l’approche prise en charge pour bloquer l’accès des utilisateurs à Yammer, voir [Désactiver l’accès à Yammer pour les utilisateurs de Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="8d2c2-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="8d2c2-107">Pour résoudre ce problème dans le portail Azure et restaurer l’accès des utilisateurs à Yammer :</span><span class="sxs-lookup"><span data-stu-id="8d2c2-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="8d2c2-108">Ouvrez la page Azure Active Directory, puis sélectionnez **Applications d’entreprise** sous **Gérer** dans le volet de navigation gauche.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="8d2c2-109">Tapez **Office 365 Yammer** dans la zone de recherche, puis sélectionnez le nom de l’application pour ouvrir les paramètres.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="8d2c2-110">Sélectionnez **Propriétés** sous **Gérer** dans le volet de navigation gauche.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="8d2c2-111">Définissez la valeur de **Activé pour que les utilisateurs se connectent ?** sur **Oui**, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="8d2c2-112">Reconnectez-vous à Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-112">Sign in to Yammer again.</span></span> <span data-ttu-id="8d2c2-113">Il se peut que vous deviez effacer les cookies.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-113">You might need to clear cookies.</span></span>

<span data-ttu-id="8d2c2-114">Vous pouvez également exécuter les commandes PowerShell pour définir la valeur.</span><span class="sxs-lookup"><span data-stu-id="8d2c2-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="8d2c2-115">Pour plus d’informations, voir [Erreur « Désolé, nous n'avons pas pu vous connecter. » lorsque vous cliquez sur la vignette Yammer dans Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="8d2c2-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 