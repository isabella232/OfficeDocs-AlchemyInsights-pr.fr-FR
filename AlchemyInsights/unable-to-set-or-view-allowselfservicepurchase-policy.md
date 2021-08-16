---
title: Impossible de définir ou d’afficher la stratégie AllowSelfServicePurchase
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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020190"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Impossible de définir ou d’afficher la stratégie AllowSelfServicePurchase

Lorsque vous tentez de définir ou d’afficher la stratégie AllowSelfServicePurchase, vous recevez le message d’erreur suivant :

*HandleError : Échec de la récupération de la stratégie de produit avec PolicyId « AllowSelfServicePurchase » et ErrorMessage : la connexion sous-jacente a été fermée : une erreur inattendue s’est produite lors d’un envoi.*

Cela peut être dû à une version antérieure de TLS (Transport Layer Security). Pour connecter le service MSCommerce, vous devez utiliser TLS 1.2 ou supérieur.  

Essayez les étapes suivantes pour activer/définir le protocole TLS sur 1.2, vérifier et réessayer.
 1. À l’invite de commandes PowerShell (PS C : entrez la commande suivante pour définir le protocole \) TLS sur la version 1.2 :

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Vérifiez le(s) protocole(s) TLS en cours d’utilisation, avec la commande suivante :

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Réessayez les commandes Obtenir ou mettre à jour si nécessaire.

