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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="bfb86-102">Résoudre des problèmes de codes d’erreur Azure AD Authentification et d’autorisation</span><span class="sxs-lookup"><span data-stu-id="bfb86-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="bfb86-103">Pour résoudre les codes d’erreur Azure AD Authentification et d’autorisation, effectuez les étapes recommandées suivantes :</span><span class="sxs-lookup"><span data-stu-id="bfb86-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="bfb86-104">**Gestion des codes d’erreur dans votre application**</span><span class="sxs-lookup"><span data-stu-id="bfb86-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="bfb86-105">La **spécifications OAuth2.0**, https://tools.ietf.org/html/rfc6749#section-5.2, fournit des instructions sur la façon de gérer les erreurs lors de l’authentification à l’aide de la partie d’erreur de la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="bfb86-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="bfb86-106">**erreur** : chaîne de code d’erreur qui peut être utilisée pour classifier les types d’erreurs qui se produisent et qui doit être utilisée pour réagir aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="bfb86-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="bfb86-107">Le champ **erreur** peut avoir plusieurs valeurs possibles. Pour plus d’informations sur les erreurs spécifiques et la manière de les corriger, voir les liens de documentation du protocole et les spécifications OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="bfb86-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="bfb86-108">Voici un exemple de réponse à une erreur :</span><span class="sxs-lookup"><span data-stu-id="bfb86-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="bfb86-109">**Recherche d'informations sur le code d'erreur actuel**</span><span class="sxs-lookup"><span data-stu-id="bfb86-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="bfb86-110">Les codes d’erreur et les messages peuvent être modifiés.</span><span class="sxs-lookup"><span data-stu-id="bfb86-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="bfb86-111">Pour consulter les informations les plus actuelles, consultez la page https://login.microsoftonline.com/error pour trouver des descriptions des erreurs AADSTS, des correctifs et quelques solutions de contournement suggérées.</span><span class="sxs-lookup"><span data-stu-id="bfb86-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="bfb86-112">Vous pouvez également rechercher et résoudre des problèmes de [codes d’erreur AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) répertoriés dans l’article [Codes d’erreur Azure AD Authentification et d’autorisation](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="bfb86-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="bfb86-113">**Obtenir de l’aide**</span><span class="sxs-lookup"><span data-stu-id="bfb86-113">**Get Help**</span></span>

- <span data-ttu-id="bfb86-114">[Options de support et d’aide pour les développeurs](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) : si vous avez besoin d’une réponse à une question ou de l’aide pour résoudre un problème qui n’est pas abordé dans notre documentation, vous pouvez demander de l’aide aux experts.</span><span class="sxs-lookup"><span data-stu-id="bfb86-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="bfb86-115">Cet article fournit plusieurs suggestions pour obtenir des réponses à vos questions à mesure que vous développez des applications qui s’intègrent à la plateforme d’identité Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bfb86-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








