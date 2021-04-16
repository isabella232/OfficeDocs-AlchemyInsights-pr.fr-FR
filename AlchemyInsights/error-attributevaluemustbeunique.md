---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813758"
---
# <a name="error-attributevaluemustbeunique"></a>Erreur : AttributeValueMustBeUnique

La raison la plus courante de l’erreur AttributeValueMustBeUnique est que deux objets avec différents SourceAnchor (immutableId) ont la même valeur pour les attributs ProxyAddresses et/ou UserPrincipalName. Pour corriger l’erreur AttributeValueMustBeUnique :
  
1. Identifiez les adresses proxyAddresses dupliquées, userPrincipalName ou toute autre valeur d’attribut à l’origine de l’erreur. Identifiez également les deux (ou plusieurs) objets impliqués dans le conflit. Le rapport généré par Azure AD Connect Health pour la synchronisation peut vous aider à identifier les deux objets.
    
2. Identifiez l’objet qui doit continuer à avoir la valeur dupliquée et l’objet qui ne doit pas l’être.
    
3. Supprimez la valeur dupliquée de l’objet qui ne doit PAS avoir cette valeur. Notez que vous devez apporter la modification dans le répertoire d’où l’objet est issu. Dans certains cas, vous devrez peut-être supprimer l’un des objets en conflit.
    
4. Si vous avez apporté la modification dans l’AD local, laissez Azure AD Connect synchroniser la modification pour que l’erreur soit corrigée.
    

