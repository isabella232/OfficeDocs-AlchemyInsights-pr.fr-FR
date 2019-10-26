---
title: Erreur AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36526988"
---
# <a name="error-attributevaluemustbeunique"></a>Erreur : AttributeValueMustBeUnique

La raison la plus fréquente de l’erreur AttributeValueMustBeUnique est que deux objets avec des ancre source (immutableId) différents ont la même valeur pour les attributs ProxyAddresses et/ou UserPrincipalName. Pour corriger l’erreur AttributeValueMustBeUnique :
  
1. Identifiez la valeur d’attribut proxyAddresses, userPrincipalName ou autre qui est à l’origine de l’erreur. Identifiez également les deux (ou plusieurs) objets impliqués dans le conflit. Le rapport généré par Azure AD Connect Health for Sync peut vous aider à identifier les deux objets.
    
2. Identifiez l’objet qui doit continuer à avoir la valeur dupliquée et l’objet ne doit pas l’être.
    
3. Supprimez la valeur dupliquée de l’objet qui ne doit pas avoir cette valeur. Notez que vous devez procéder à la modification dans le répertoire à partir duquel l’objet est source. Dans certains cas, vous devrez peut-être supprimer l’un des objets en conflit.
    
4. Si vous avez effectué la modification dans l’AD locale, laissez Azure AD Connect synchroniser la modification pour l’erreur afin d’obtenir des fixes.
    

