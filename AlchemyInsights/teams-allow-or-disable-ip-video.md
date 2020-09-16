---
title: Teams autorise ou désactive la vidéo IP
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
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670182"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams autorise ou désactive la vidéo IP

**Modifier ou créer une stratégie de réunion**

Pour modifier ou créer une stratégie de réunion, accédez au **Centre d’administration Microsoft Teams > Réunions > Stratégies de réunion**. Sélectionnez une stratégie dans la liste ou cliquez sur **Ajouter**. Si vous créez une stratégie, ajoutez un nom et une description. Le nom ne peut pas contenir de caractères spéciaux et ne doit pas dépasser 64 caractères. Choisissez les paramètres, puis cliquez sur **Enregistrer**.

Par exemple, imaginons que vous avez de nombreux d’utilisateurs et que vous voulez limiter la quantité de bande passante requise par la réunion. Vous devez créer une stratégie personnalisée nommée « bande passante limitée » et désactiver les paramètres suivants :

Sous ** Audio & vidéo** :

- Désactivez l’option Autoriser l’enregistrement Cloud.
- Désactivez Autoriser la vidéo IP.

Vous pouvez ensuite attribuer la stratégie aux utilisateurs.

**Affecter une stratégie de réunion aux utilisateurs**

1. Dans le volet de navigation gauche du centre d’administration Microsoft Teams, et accédez aux **Utilisateurs**, puis cliquez sur l’utilisateur.
2. Sélectionnez l’utilisateur en cliquant à gauche du nom de celui-ci, puis cliquez sur **Modifier les paramètres**.
3. Sous **Stratégie de réunion**, sélectionnez la stratégie que vous souhaitez attribuer, et puis cliquez sur **Appliquer**.

Si vous souhaitez obtenir plus d’informations, voir [Gérer les stratégies de réunion dans Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
