---
title: Comportement consistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816990"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="018e8-102">Comportement consistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="018e8-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="018e8-103">Azure AD Connect (version 1.1.524.0 et versions antérieures) facilite désormais l'utilisation de msDS-ConsistencyGuid comme attribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="018e8-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="018e8-104">Lorsque vous utilisez cette fonctionnalité, Azure AD Connect configure automatiquement les règles de synchronisation pour :</span><span class="sxs-lookup"><span data-stu-id="018e8-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="018e8-105">Utilisez msDS-ConsistencyGuid comme attribut sourceAnchor pour les objets User.</span><span class="sxs-lookup"><span data-stu-id="018e8-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="018e8-106">ObjectGUID est utilisé pour d'autres types d'objets.</span><span class="sxs-lookup"><span data-stu-id="018e8-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="018e8-107">Pour tout objet AD User local donné dont l'attribut msDS-ConsistencyGuid n'est pas rempli, Azure AD Connect écrit sa valeur objectGUID dans l'attribut msDS-ConsistencyGuid dans Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="018e8-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="018e8-108">Une fois l'attribut msDS-ConsistencyGuid rempli, Azure AD Connect exporte l'objet vers Azure AD.</span><span class="sxs-lookup"><span data-stu-id="018e8-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="018e8-109">**Remarque :** Une fois qu'un objet AD local est importé dans Azure AD Connect (c'est-à-dire importé dans l'espace connecteur AD et projeté dans le métaverse), vous ne pouvez plus modifier sa valeur sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="018e8-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="018e8-110">Pour spécifier la valeur sourceAnchor pour un objet AD local donné, configurez son attribut msDS-ConsistencyGuid avant qu'il ne soit importé dans Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="018e8-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="018e8-111">Pour plus d'informations sur SourceAnchor et ConsistencyGuid, reportez-vous aux concepts suivants : [Azure AD Connect : concepts de conception](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="018e8-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

