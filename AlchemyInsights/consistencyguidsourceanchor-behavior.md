---
title: Comportement ConsistencyGuid/ancre source
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516977"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f2b6c-102">Comportement ConsistencyGuid/ancre source</span><span class="sxs-lookup"><span data-stu-id="f2b6c-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f2b6c-103">Azure AD Connect (version 1.1.524.0 et after) facilite désormais l’utilisation de msDS-ConsistencyGuid en tant qu’attribut ancre source.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="f2b6c-104">Lors de l’utilisation de cette fonctionnalité, Azure AD Connect configure automatiquement les règles de synchronisation de la manière suivante :</span><span class="sxs-lookup"><span data-stu-id="f2b6c-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f2b6c-105">Utilisez msDS-ConsistencyGuid comme attribut ancre source pour les objets utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="f2b6c-106">ObjectGUID est utilisé pour d’autres types d’objets.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f2b6c-107">Pour tout objet utilisateur AD local donné dont l’attribut msDS-ConsistencyGuid n’est pas rempli, Azure AD Connect écrit sa valeur objectGUID dans l’attribut msDS-ConsistencyGuid dans Active Directory sur site.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="f2b6c-108">Une fois que l’attribut msDS-ConsistencyGuid est rempli, Azure AD Connect exporte l’objet vers Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f2b6c-109">**Remarque :** Une fois qu’un objet AD local est importé dans Azure AD Connect (c’est-à-dire, importé dans l’espace AD Connector et projeté dans le métaverse), vous ne pouvez plus modifier sa valeur ancre source.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="f2b6c-110">Pour spécifier la valeur ancre source pour un objet AD local donné, configurez son attribut msDS-ConsistencyGuid avant de l’importer dans Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f2b6c-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f2b6c-111">Pour plus d’informations sur ancre source et ConsistencyGuid, reportez-vous à la rubrique suivante : [Azure ad Connect : Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f2b6c-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

