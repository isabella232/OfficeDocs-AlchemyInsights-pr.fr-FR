---
title: Impossible de définir ou d'afficher la stratégie AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826089"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="77e7f-102">Impossible de définir ou d'afficher la stratégie AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="77e7f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="77e7f-103">Lorsque vous tentez de définir ou d'afficher la stratégie AllowSelfServicePurchase, vous recevez le message d'erreur suivant :</span><span class="sxs-lookup"><span data-stu-id="77e7f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="77e7f-104">*HandleError : Échec de la récupération de la stratégie de produit avec PolicyId « AllowSelfServicePurchase » et ErrorMessage : la connexion sous-jacente a été fermée : une erreur inattendue s'est produite lors d'un envoi.*</span><span class="sxs-lookup"><span data-stu-id="77e7f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="77e7f-105">Cela peut être dû à une version antérieure de TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="77e7f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="77e7f-106">Pour connecter le service MSCommerce, vous devez utiliser TLS 1.2 ou supérieur.</span><span class="sxs-lookup"><span data-stu-id="77e7f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="77e7f-107">Essayez les étapes suivantes pour activer/définir le protocole TLS sur 1.2, vérifier et réessayer.</span><span class="sxs-lookup"><span data-stu-id="77e7f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="77e7f-108">À l'invite de commandes PowerShell (PS C : entrez la commande suivante pour définir le protocole \) TLS sur la version 1.2 :</span><span class="sxs-lookup"><span data-stu-id="77e7f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="77e7f-109">Vérifiez le(s) protocole(s) TLS en cours d'utilisation, avec la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="77e7f-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="77e7f-110">Réessayez les commandes Obtenir ou mettre à jour si nécessaire.</span><span class="sxs-lookup"><span data-stu-id="77e7f-110">Retry the Get or Update commands as needed.</span></span>

