---
title: Lecture seule pour un message de maintenance lors de la tentative d’utilisation de SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670830"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="359ee-102">Lecture seule pour un message de maintenance lors de la tentative d’utilisation de SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="359ee-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="359ee-103">Les utilisateurs peuvent recevoir un message **de maintenance en lecture seule** lorsqu’ils tentent d’utiliser SharePoint ou OneDrive pour l’un des scénarios suivants.</span><span class="sxs-lookup"><span data-stu-id="359ee-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="359ee-104">Activité de maintenance planifiée ou active.</span><span class="sxs-lookup"><span data-stu-id="359ee-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="359ee-105">Vérifiez-les en accédant au [Centre de messages](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="359ee-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="359ee-106">Un incident de service actif de haute priorité susceptible de se produire.</span><span class="sxs-lookup"><span data-stu-id="359ee-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="359ee-107">Recherchez les avis/incidents en accédant à l' [État du service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="359ee-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="359ee-108">Un scénario de récupération de réparation automatique mineur qui peut être dû à des événements inattendus sur les serveurs qui peuvent durer moins de 30 minutes ou plus.</span><span class="sxs-lookup"><span data-stu-id="359ee-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="359ee-109">Il n’existe aucune publication de centre de messages ou d’intégrité de service pour ces récupérateurs mineurs, mais vous devriez être redirigé vers la version normale très prochainement.</span><span class="sxs-lookup"><span data-stu-id="359ee-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="359ee-110">En très peu de occasions, nous avons observé que l’un des trois scénarios mentionnés ci-dessus était la cause, et que le service a été restauré, mais que le cache du navigateur des utilisateurs n’a pas été effacé.</span><span class="sxs-lookup"><span data-stu-id="359ee-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="359ee-111">Essayez de vider le cache du navigateur avant de naviguer sur le site.</span><span class="sxs-lookup"><span data-stu-id="359ee-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="359ee-112">Dans votre navigateur Microsoft Edge, sélectionnez **paramètres**, puis **confidentialité et sécurité**.</span><span class="sxs-lookup"><span data-stu-id="359ee-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="359ee-113">Sous **effacer la navigation**, sélectionnez **choisir les éléments à effacer**.</span><span class="sxs-lookup"><span data-stu-id="359ee-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="359ee-114">Sélectionnez **cookies et données de site Web enregistrées**, puis sélectionnez **Effacer**.</span><span class="sxs-lookup"><span data-stu-id="359ee-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="359ee-115">Ces étapes peuvent varier en cas d’utilisation d’autres navigateurs, tels que Mozilla Firefox ou Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="359ee-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="359ee-116">Une autre option consiste à ouvrir votre site SharePoint ou OneDrive dans une nouvelle fenêtre InPrivate.</span><span class="sxs-lookup"><span data-stu-id="359ee-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>