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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002118"
---
# <a name="error-attributevaluemustbeunique"></a>Erreur : AttributeValueMustBeUnique

La raison la plus courante de l’erreur AttributeValueMustBeUnique est que deux objets avec différents SourceAnchor (immutableId) ont la même valeur pour les attributs ProxyAddresses et/ou UserPrincipalName. Pour corriger l’erreur AttributeValueMustBeUnique :
  
1. Identifiez les adresses proxyAddresses dupliquées, userPrincipalName ou toute autre valeur d’attribut à l’origine de l’erreur. Identifiez également les deux (ou plusieurs) objets impliqués dans le conflit. Le rapport généré par Azure AD Connecter Health for sync peut vous aider à identifier les deux objets.
    
2. Identifiez l’objet qui doit continuer à avoir la valeur dupliquée et l’objet qui ne doit pas l’être.
    
3. Supprimez la valeur dupliquée de l’objet qui ne doit PAS avoir cette valeur. Notez que vous devez apporter la modification dans le répertoire d’où l’objet est issu. Dans certains cas, vous devrez peut-être supprimer l’un des objets en conflit.
    
4. Si vous avez apporté la modification dans l’AD local, laissez Azure AD Connecter synchroniser la modification pour que l’erreur soit corrigée.
    

