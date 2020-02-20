---
title: Impossible de définir ou d’afficher la stratégie AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158559"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="94437-102">Impossible de définir ou d’afficher la stratégie AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="94437-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="94437-103">Lors de la tentative de définition ou d’affichage de la stratégie AllowSelfServicePurchase, vous recevez le message d’erreur suivant :</span><span class="sxs-lookup"><span data-stu-id="94437-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="94437-104">*HandleError : échec de la récupération de la stratégie de produit avec PolicyId’AllowSelfServicePurchase', ErrorMessage-la connexion sous-jacente a été fermée : une erreur inattendue s’est produite lors de l’envoi.*</span><span class="sxs-lookup"><span data-stu-id="94437-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="94437-105">Cela peut être dû à une version plus ancienne de TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="94437-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="94437-106">Pour connecter le service MSCommerce, vous devez utiliser TLS 1,2 ou une version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="94437-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="94437-107">Procédez comme suit pour activer/définir le protocole TLS sur 1,2, vérifiez et recommencez.</span><span class="sxs-lookup"><span data-stu-id="94437-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="94437-108">À l’invite de commandes PowerShell (PS C\) : entrez la commande suivante pour définir le protocole TLS sur la version 1,2 :</span><span class="sxs-lookup"><span data-stu-id="94437-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="94437-109">Vérifiez que les protocoles TLS sont utilisés, à l’aide de la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="94437-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="94437-110">Recommencez les commandes obtenir ou mettre à jour selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="94437-110">Retry the Get or Update commands as needed.</span></span>

