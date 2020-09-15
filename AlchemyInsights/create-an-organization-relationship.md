---
title: Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712731"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="21b71-102">Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation</span><span class="sxs-lookup"><span data-stu-id="21b71-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="21b71-103">À partir du tableau de bord du Centre d’administration Microsoft 365, accédez à **Administrateur** > \*\* Exchange\*\*.</span><span class="sxs-lookup"><span data-stu-id="21b71-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="21b71-104">Accédez à **organisation** > **partage**.</span><span class="sxs-lookup"><span data-stu-id="21b71-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="21b71-105">Sous **Partage d’organisation**, cliquez sur **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="21b71-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="21b71-106">Dans **Nouvelle relation organisationnelle**, dans la boîte de dialogue **Nom de la relation**, entrez un nom convivial pour la relation d'organisation.</span><span class="sxs-lookup"><span data-stu-id="21b71-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="21b71-p101">Dans la zone **Domaines à partager avec**, tapez le domaine de l'organisation Office 365 externe ou Exchange sur site à laquelle vous voulez donner accès à vos calendriers. Pour entrer plusieurs domaines, séparez les noms de domaine par une virgule. Par exemple, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="21b71-p101">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars. If you need to enter more than one domain, separate the domain names with a comma. For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="21b71-p102">Cochez la case **Activer le partage des informations de disponibilité de calendrier** pour activer le partage de calendrier avec les domaines que vous avez répertoriés. Définissez le niveau de partage des informations de disponibilité du calendrier, ainsi que les utilisateurs pouvant partager ces informations.</span><span class="sxs-lookup"><span data-stu-id="21b71-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="21b71-112">Pour définir le niveau d'accès de la disponibilité, sélectionnez l'une des opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="21b71-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="21b71-113">**Informations de disponibilité de calendrier avec les heures de disponibilité uniquement**</span><span class="sxs-lookup"><span data-stu-id="21b71-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="21b71-114">**Disponibilité de calendrier avec l’heure, l'objet et emplacement**</span><span class="sxs-lookup"><span data-stu-id="21b71-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="21b71-115">Pour définir les utilisateurs qui partagent des informations de disponibilité de calendrier, sélectionnez l'une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="21b71-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="21b71-116">**Tout le monde dans votre organisation**</span><span class="sxs-lookup"><span data-stu-id="21b71-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="21b71-117">**Un groupe de sécurité spécifié**</span><span class="sxs-lookup"><span data-stu-id="21b71-117">**A specified security group**</span></span>  

<span data-ttu-id="21b71-118">Cliquez sur **Parcourir** pour sélectionner un groupe de sécurité dans la liste, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="21b71-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="21b71-119">Cliquez sur **Enregistrer** pour créer la relation organisationnelle.</span><span class="sxs-lookup"><span data-stu-id="21b71-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="21b71-120">**Remarque :** les configurations inter-clients ne prennent pas en charge les contacts personnels pour la recherche de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="21b71-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="21b71-121">Vous devez inclure les contacts dans la liste d’adresses globale pour que la recherche de disponibilité fonctionne.</span><span class="sxs-lookup"><span data-stu-id="21b71-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="21b71-122">**Pour une compréhension complète de ce sujet, veuillez consulter :**</span><span class="sxs-lookup"><span data-stu-id="21b71-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="21b71-123">Créer une relation d’organisation dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="21b71-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="21b71-124">Modifier une relation d’organisation dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="21b71-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="21b71-125">Supprimer une relation d’organisation dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="21b71-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
