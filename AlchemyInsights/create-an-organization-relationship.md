---
title: Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816126"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="0ee2c-102">Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation</span><span class="sxs-lookup"><span data-stu-id="0ee2c-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="0ee2c-103">À partir du tableau de bord du Centre d’administration Microsoft 365, accédez à **Administrateur** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="0ee2c-104">Accédez à **organisation** > **partage**.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="0ee2c-105">Sous **Partage d’organisation**, cliquez sur **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="0ee2c-106">Dans **Nouvelle relation organisationnelle**, dans la boîte de dialogue **Nom de la relation**, entrez un nom convivial pour la relation d'organisation.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="0ee2c-p101">Dans la zone **Domaines à partager avec**, tapez le domaine de l'organisation Office 365 externe ou Exchange sur site à laquelle vous voulez donner accès à vos calendriers. Pour entrer plusieurs domaines, séparez les noms de domaine par une virgule. Par exemple, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-p101">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars. If you need to enter more than one domain, separate the domain names with a comma. For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="0ee2c-p102">Cochez la case **Activer le partage des informations de disponibilité de calendrier** pour activer le partage de calendrier avec les domaines que vous avez répertoriés. Définissez le niveau de partage des informations de disponibilité du calendrier, ainsi que les utilisateurs pouvant partager ces informations.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="0ee2c-112">Pour définir le niveau d'accès de la disponibilité, sélectionnez l'une des opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="0ee2c-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="0ee2c-113">**Informations de disponibilité de calendrier avec les heures de disponibilité uniquement**</span><span class="sxs-lookup"><span data-stu-id="0ee2c-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="0ee2c-114">**Disponibilité de calendrier avec l’heure, l'objet et emplacement**</span><span class="sxs-lookup"><span data-stu-id="0ee2c-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="0ee2c-115">Pour définir les utilisateurs qui partagent des informations de disponibilité de calendrier, sélectionnez l'une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="0ee2c-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="0ee2c-116">**Tout le monde dans votre organisation**</span><span class="sxs-lookup"><span data-stu-id="0ee2c-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="0ee2c-117">**Un groupe de sécurité spécifié**</span><span class="sxs-lookup"><span data-stu-id="0ee2c-117">**A specified security group**</span></span>  

<span data-ttu-id="0ee2c-118">Cliquez sur **Parcourir** pour sélectionner un groupe de sécurité dans la liste, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="0ee2c-119">Cliquez sur **Enregistrer** pour créer la relation organisationnelle.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="0ee2c-120">**Remarque :** les configurations inter-clients ne prennent pas en charge les contacts personnels pour la recherche de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="0ee2c-121">Vous devez inclure les contacts dans la liste d’adresses globale pour que la recherche de disponibilité fonctionne.</span><span class="sxs-lookup"><span data-stu-id="0ee2c-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="0ee2c-122">**Pour une compréhension complète de ce sujet, veuillez consulter :**</span><span class="sxs-lookup"><span data-stu-id="0ee2c-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="0ee2c-123">Créer une relation d’organisation dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="0ee2c-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="0ee2c-124">Modifier une relation d’organisation dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="0ee2c-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="0ee2c-125">Supprimer une relation d’organisation dans Exchange Online</span><span class="sxs-lookup"><span data-stu-id="0ee2c-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
