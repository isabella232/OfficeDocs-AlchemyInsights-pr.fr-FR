---
title: ConsistencyGuid / comportement sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498516"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="5feb4-102">ConsistencyGuid / comportement sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="5feb4-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="5feb4-p101">Azure AD Connect (version 1.1.524.0 et après) autorise l’utilisation de l’attribut msDS-ConsistencyGuid en tant qu’attribut sourceAnchor. Lorsque vous utilisez cette fonctionnalité, Azure AD Connect configure automatiquement les règles de synchronisation pour :</span><span class="sxs-lookup"><span data-stu-id="5feb4-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="5feb4-p102">Utilisez msDS-ConsistencyGuid en tant que l’attribut sourceAnchor pour les objets utilisateur. GUID d’objet est utilisée pour d’autres types d’objet.</span><span class="sxs-lookup"><span data-stu-id="5feb4-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="5feb4-p103">Des locaux utilisateur AD objet dont l’attribut msDS-ConsistencyGuid n’est pas remplies, Azure écritures AD Connect sa valeur GUID d’objet sauvegarder à l’attribut msDS-ConsistencyGuid sur site Active Directory. Une fois que l’attribut msDS-ConsistencyGuid est rempli, Azure AD Connect exporte ensuite l’objet dans Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5feb4-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="5feb4-p104">**Remarque :** Une fois sur site objet AD est importé dans Azure Connect AD (c'est-à-dire, importé dans l’espace connecteur AD et projeté dans le métaverse), vous ne pouvez pas modifier sa valeur sourceAnchor plus. Pour spécifier la valeur sourceAnchor pour une donnée sur site AD d’objet, configurer son attribut msDS-ConsistencyGuid avant qu’il est importé dans Azure AD se connecter.</span><span class="sxs-lookup"><span data-stu-id="5feb4-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="5feb4-111">Pour plus d’informations sur SourceAnchor et ConsistencyGuid, reportez-vous aux ressources suivantes : [Azure AD Connect : concepts de conception](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="5feb4-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

