---
title: Le courrier électronique de flux de travail n’est pas envoyé
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766131"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a1058-102">Le courrier de flux de travail n’est pas envoyé pour une liste ou une bibliothèque SharePoint</span><span class="sxs-lookup"><span data-stu-id="a1058-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a1058-103">Les courriers électroniques provenant de flux de travail ne sont pas envoyés à tous les utilisateurs ou uniquement à des utilisateurs spécifiques, ou vous voyez l’erreur que **le message électronique ne peut pas être envoyé. Assurez-vous que le message électronique contient un destinataire valide**.</span><span class="sxs-lookup"><span data-stu-id="a1058-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a1058-104">Vérifiez si l’utilisateur existe dans le groupe d’autorisations **tous les personnes** (liste d’informations utilisateur) pour cette collection de sites.</span><span class="sxs-lookup"><span data-stu-id="a1058-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a1058-105">Exemple d’URL directe :<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx ? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="a1058-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a1058-106">Si l’utilisateur n’existe pas, vérifiez que l’utilisateur est connecté à la page.</span><span class="sxs-lookup"><span data-stu-id="a1058-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a1058-107">S’il s’agit d’un utilisateur externe, assurez-vous que son invitation a été acceptée.</span><span class="sxs-lookup"><span data-stu-id="a1058-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a1058-108">Si l’utilisateur existe dans le groupe d’autorisations, assurez-vous que l’adresse de messagerie est correcte.</span><span class="sxs-lookup"><span data-stu-id="a1058-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a1058-109">Si l’adresse de messagerie de l’utilisateur n’est pas définie ici, créez un exemple d’alerte pour cet utilisateur, ce qui force la synchronisation de ce compte d’utilisateur à partir des profils utilisateur de SharePoint vers cette collection de sites.</span><span class="sxs-lookup"><span data-stu-id="a1058-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a1058-110">Les courriers électroniques provenant de flux de travail sont envoyés aux administrateurs de collection de sites, mais pas aux autres utilisateurs et le message d’erreur **http interdit à <span>https :</span>//URL/_vti_bin/client.XVC.sp.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="a1058-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a1058-111">Consultez [la rubrique accès refusé lorsque vous envoyez un message électronique à un groupe SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a1058-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a1058-112">Vérifiez également que la fonctionnalité de collection de sites **mode verrouillage avec accès limité aux utilisateurs** n’est pas active.</span><span class="sxs-lookup"><span data-stu-id="a1058-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a1058-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a1058-113">Related topics</span></span>
<span data-ttu-id="a1058-114">Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?</span><span class="sxs-lookup"><span data-stu-id="a1058-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a1058-115">Créer un flux</span><span class="sxs-lookup"><span data-stu-id="a1058-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a1058-116">SharePoint et flux</span><span class="sxs-lookup"><span data-stu-id="a1058-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


