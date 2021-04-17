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
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportement consistencyGuid/sourceAnchor

Azure AD Connect (version 1.1.524.0 et versions antérieures) facilite désormais l'utilisation de msDS-ConsistencyGuid comme attribut sourceAnchor. Lorsque vous utilisez cette fonctionnalité, Azure AD Connect configure automatiquement les règles de synchronisation pour :
  
- Utilisez msDS-ConsistencyGuid comme attribut sourceAnchor pour les objets User. ObjectGUID est utilisé pour d'autres types d'objets.
    
- Pour tout objet AD User local donné dont l'attribut msDS-ConsistencyGuid n'est pas rempli, Azure AD Connect écrit sa valeur objectGUID dans l'attribut msDS-ConsistencyGuid dans Active Directory local. Une fois l'attribut msDS-ConsistencyGuid rempli, Azure AD Connect exporte l'objet vers Azure AD.
    
 **Remarque :** Une fois qu'un objet AD local est importé dans Azure AD Connect (c'est-à-dire importé dans l'espace connecteur AD et projeté dans le métaverse), vous ne pouvez plus modifier sa valeur sourceAnchor. Pour spécifier la valeur sourceAnchor pour un objet AD local donné, configurez son attribut msDS-ConsistencyGuid avant qu'il ne soit importé dans Azure AD Connect. 
  
Pour plus d'informations sur SourceAnchor et ConsistencyGuid, reportez-vous aux concepts suivants : [Azure AD Connect : concepts de conception](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

