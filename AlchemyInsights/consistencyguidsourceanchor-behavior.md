---
title: ConsistencyGuid / comportement sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927640"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / comportement sourceAnchor

Azure AD Connect (version 1.1.524.0 et après) autorise l’utilisation de l’attribut msDS-ConsistencyGuid en tant qu’attribut sourceAnchor. Lorsque vous utilisez cette fonctionnalité, Azure AD Connect configure automatiquement les règles de synchronisation pour :
  
- Utilisez msDS-ConsistencyGuid en tant que l’attribut sourceAnchor pour les objets utilisateur. GUID d’objet est utilisée pour d’autres types d’objet.
    
- Des locaux utilisateur AD objet dont l’attribut msDS-ConsistencyGuid n’est pas remplies, Azure écritures AD Connect sa valeur GUID d’objet sauvegarder à l’attribut msDS-ConsistencyGuid sur site Active Directory. Une fois que l’attribut msDS-ConsistencyGuid est rempli, Azure AD Connect exporte ensuite l’objet dans Azure AD.
    
 **Remarque :** Une fois sur site objet AD est importé dans Azure Connect AD (c'est-à-dire, importé dans l’espace connecteur AD et projeté dans le métaverse), vous ne pouvez pas modifier sa valeur sourceAnchor plus. Pour spécifier la valeur sourceAnchor pour une donnée sur site AD d’objet, configurer son attribut msDS-ConsistencyGuid avant qu’il est importé dans Azure AD se connecter. 
  
Pour plus d’informations sur SourceAnchor et ConsistencyGuid, reportez-vous aux ressources suivantes : [Azure AD Connect : concepts de conception](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

