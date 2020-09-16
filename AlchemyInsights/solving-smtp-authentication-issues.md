---
title: Résolution des problèmes d’authentification SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737987"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="68f0d-102">Résolution des problèmes d’authentification SMTP</span><span class="sxs-lookup"><span data-stu-id="68f0d-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="68f0d-103">Si vous rencontrez des erreurs 5.7.57 ou 5.7.3 lorsque vous essayez d’envoyer des courriers électroniques SMTP et de vous authentifier auprès d’un client ou d’une application, il existe quelques points que vous devez vérifier :</span><span class="sxs-lookup"><span data-stu-id="68f0d-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="68f0d-104">Il est possible que l’envoi SMTP authentifié soit désactivé dans votre client, ou sur la boîte aux lettres que vous essayez d’utiliser (vérifiez les deux paramètres).</span><span class="sxs-lookup"><span data-stu-id="68f0d-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="68f0d-105">Pour en savoir plus, voir [Activer ou désactiver l’envoi SMTP du client authentifié](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="68f0d-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="68f0d-106">Vérifiez si les [Valeurs par défaut d’Azure Security](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) sont activées pour votre client. Si l’option est activée, l’authentification SMTP à l’aide de l’authentification de base (également connue sous le nom de héritage ; celle-ci utilisera un nom d’utilisateur et un mot de passe) échouera.</span><span class="sxs-lookup"><span data-stu-id="68f0d-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
