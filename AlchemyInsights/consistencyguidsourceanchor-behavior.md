---
title: Comportement ConsistencyGuid/ancre source
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756281"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportement ConsistencyGuid/ancre source

Azure AD Connect (version 1.1.524.0 et after) facilite désormais l’utilisation de msDS-ConsistencyGuid en tant qu’attribut ancre source. Lors de l’utilisation de cette fonctionnalité, Azure AD Connect configure automatiquement les règles de synchronisation de la manière suivante :
  
- Utilisez msDS-ConsistencyGuid comme attribut ancre source pour les objets utilisateur. ObjectGUID est utilisé pour d’autres types d’objets.
    
- Pour tout objet utilisateur AD local donné dont l’attribut msDS-ConsistencyGuid n’est pas rempli, Azure AD Connect écrit sa valeur objectGUID dans l’attribut msDS-ConsistencyGuid dans Active Directory sur site. Une fois que l’attribut msDS-ConsistencyGuid est rempli, Azure AD Connect exporte l’objet vers Azure AD.
    
 **Remarque :** Une fois qu’un objet AD local est importé dans Azure AD Connect (c’est-à-dire, importé dans l’espace AD Connector et projeté dans le métaverse), vous ne pouvez plus modifier sa valeur ancre source. Pour spécifier la valeur ancre source pour un objet AD local donné, configurez son attribut msDS-ConsistencyGuid avant de l’importer dans Azure AD Connect. 
  
Pour plus d’informations sur ancre source et ConsistencyGuid, reportez-vous à la rubrique suivante : [Azure ad Connect : Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

