---
title: 2491 Alerte des messages électroniques à partir de la stratégie « Hameçonnage remis en raison d’un remplacement par le client ou l’utilisateur »
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e24f489292f38b5e9cacc8b9bfe5730ebfc71ce5e3004be479134ef6c791a12
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899330"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alerte des messages électroniques à partir de la stratégie « Hameçonnage remis en raison d’un remplacement par le client ou l’utilisateur »

Une stratégie d’alerte par défaut nommée **Phish Delivered** en raison d’un remplacement par le client ou l’utilisateur est disponible dans les organisations avec Microsoft Defender pour Office 365 licences P1 et P2. Si vous avez reçu cette alerte, voici les étapes à suivre pour examiner :

1. Dans le message d’alerte, cliquez **sur Afficher** l’alerte pour aller à la page **Alertes** dans Microsoft 365 Defender portail.

2. Sélectionnez l’alerte pour afficher l’option Afficher la liste **des messages** ou Afficher les messages **dans l’Explorateur.** Ces deux options vous prennent en compte pour obtenir les détails du message, notamment l’ID de message. Notez que le lien Explorateur de menaces filtre automatiquement les messages qui correspondent aux critères d’alerte. Vous devrez peut-être ajuster le filtre de date dans l’Explorateur de menaces.

Le message d’hameçonnage a été remis en raison d’une substitution configurée manuellement :

- Expéditeur ou domaine autorisé par l’utilisateur.
- Expéditeur ou domaine autorisé par l’administrateur dans une stratégie anti-courrier indésirable.
- Adresse IP autorisée dans une stratégie de filtrage des connexions.
- Règle de flux de messagerie (également appelée règle de transport) configurée pour autoriser les messages.

Si vous pensez que le message a [](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) été marqué à tort comme hameçonnage, utilisez la soumission de l’administrateur pour signaler le message à Microsoft.

Les utilisateurs peuvent utiliser [le add-in Signaler](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) un message ou le Outlook signaler le hameçonnage pour envoyer des exemples de message à Microsoft.
