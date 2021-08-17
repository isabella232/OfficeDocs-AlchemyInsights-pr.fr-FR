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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044338"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportement consistencyGuid/sourceAnchor

Azure AD Connecter (version 1.1.524.0 et versions antérieures) facilite désormais l’utilisation de msDS-ConsistencyGuid comme attribut sourceAnchor. Lorsque vous utilisez cette fonctionnalité, Azure AD Connecter configure automatiquement les règles de synchronisation pour :
  
- Utilisez msDS-ConsistencyGuid comme attribut sourceAnchor pour les objets User. ObjectGUID est utilisé pour d’autres types d’objets.
    
- Pour tout objet AD User local donné dont l’attribut msDS-ConsistencyGuid n’est pas rempli, Azure AD Connecter écrit sa valeur objectGUID dans l’attribut msDS-ConsistencyGuid dans Active Directory local. Une fois l’attribut msDS-ConsistencyGuid rempli, Azure AD Connecter puis exporte l’objet vers Azure AD.
    
 **Remarque :** Une fois qu’un objet AD local est importé dans Azure AD Connecter (c’est-à-dire importé dans l’espace connecteur AD et projeté dans le métaverse), vous ne pouvez plus modifier sa valeur sourceAnchor. Pour spécifier la valeur sourceAnchor pour un objet AD local donné, configurez son attribut msDS-ConsistencyGuid avant qu’il ne soit importé dans Azure AD Connecter. 
  
Pour plus d’informations sur SourceAnchor et ConsistencyGuid, reportez-vous aux informations suivantes : [Azure AD Connecter : concepts de conception](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

