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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091698"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Impossible de définir ou d’afficher la stratégie AllowSelfServicePurchase

Lors de la tentative de définition ou d’affichage de la stratégie AllowSelfServicePurchase, vous recevez le message d’erreur suivant :

*HandleError : échec de la récupération de la stratégie de produit avec PolicyId’AllowSelfServicePurchase', ErrorMessage-la connexion sous-jacente a été fermée : une erreur inattendue s’est produite lors de l’envoi.*

Cela peut être dû à une version plus ancienne de TLS (Transport Layer Security). Pour connecter le service MSCommerce, vous devez utiliser TLS 1,2 ou une version ultérieure.  

Procédez comme suit pour activer/définir le protocole TLS sur 1,2, vérifiez et recommencez.
 1. À l’invite de commandes PowerShell (PS C\) : entrez la commande suivante pour définir le protocole TLS sur la version 1,2 :

    \[NET. ServicePointManager] :: SecurityProtocol = \[net. SecurityProtocolType] :: Tls12

2. Vérifiez que les protocoles TLS sont utilisés, à l’aide de la commande suivante :

    \[NET. ServicePointManager] :: SecurityProtocol 

3. Recommencez les commandes obtenir ou mettre à jour selon vos besoins.

