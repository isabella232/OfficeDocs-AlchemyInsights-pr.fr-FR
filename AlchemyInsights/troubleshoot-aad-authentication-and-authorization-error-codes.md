---
title: Résoudre des problèmes de codes d’erreur Azure AD Authentification et d’autorisation
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897833"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Résoudre des problèmes de codes d’erreur Azure AD Authentification et d’autorisation

Pour résoudre les codes d’erreur Azure AD Authentification et d’autorisation, effectuez les étapes recommandées suivantes :

1. **Gestion des codes d’erreur dans votre application**

- La **spécifications OAuth2.0**, https://tools.ietf.org/html/rfc6749#section-5.2, fournit des instructions sur la façon de gérer les erreurs lors de l’authentification à l’aide de la partie d’erreur de la réponse aux erreurs.

    - **erreur** : chaîne de code d’erreur qui peut être utilisée pour classifier les types d’erreurs qui se produisent et qui doit être utilisée pour réagir aux erreurs.
    - Le champ **erreur** peut avoir plusieurs valeurs possibles. Pour plus d’informations sur les erreurs spécifiques et la manière de les corriger, voir les liens de documentation du protocole et les spécifications OAuth 2.0.

- Voici un exemple de réponse à une erreur :
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Recherche d'informations sur le code d'erreur actuel**

- Les codes d’erreur et les messages peuvent être modifiés. Pour consulter les informations les plus actuelles, consultez la page https://login.microsoftonline.com/error pour trouver des descriptions des erreurs AADSTS, des correctifs et quelques solutions de contournement suggérées.
- Vous pouvez également rechercher et résoudre des problèmes de [codes d’erreur AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) répertoriés dans l’article [Codes d’erreur Azure AD Authentification et d’autorisation](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Obtenir de l’aide**

- [Options de support et d’aide pour les développeurs](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) : si vous avez besoin d’une réponse à une question ou de l’aide pour résoudre un problème qui n’est pas abordé dans notre documentation, vous pouvez demander de l’aide aux experts. Cet article fournit plusieurs suggestions pour obtenir des réponses à vos questions à mesure que vous développez des applications qui s’intègrent à la plateforme d’identité Microsoft.








