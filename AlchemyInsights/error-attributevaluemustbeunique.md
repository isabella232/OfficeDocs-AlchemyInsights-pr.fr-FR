---
title: Erreur AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288346"
---
# <a name="error-attributevaluemustbeunique"></a>Erreur : AttributeValueMustBeUnique

Le plus souvent pour l’erreur AttributeValueMustBeUnique est deux objets avec différente SourceAnchor (immutableId) ont la même valeur pour les attributs ProxyAddresses et/ou UserPrincipalName. Pour corriger l’erreur AttributeValueMustBeUnique :
  
1. Identifier les proxyAddresses dupliqué, userPrincipalName ou autre valeur d’attribut qui est à l’origine de l’erreur. Identifiez également les objets deux (ou plus) sont impliqués dans le conflit. Le rapport généré par Azure AD se connecter d’intégrité pour la synchronisation peut vous aider à identifier les deux objets.
    
2. Identifier l’objet puissent continuer à la valeur double et l’objet ne doit pas.
    
3. Supprimez la valeur double de l’objet qui ne doit pas comporter de cette valeur. Notez que vous devez vous la modification dans le répertoire dans lequel l’objet est provenant de. Dans certains cas, vous devrez peut-être supprimer un des objets en conflit.
    
4. Si vous avez effectué la modification dans l’environnement local sur AD, laisser Azure AD Connect synchroniser la modification de l’erreur pour le résoudre.
    

