---
title: 2491 alerte les messages électroniques provenant de la stratégie «hameçonnage fourni suite à une substitution de client ou d’utilisateur»
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391260"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertez les messages électroniques provenant de la stratégie «hameçonnage fourni suite à une substitution de client ou d’utilisateur»

Une stratégie d’alerte par défaut nommée «hameçonnage remis en raison de la substitution du client ou de l’utilisateur» a été déployée pour les locataires ayant des licences P1 et P2 Office 365 ATP. Si vous avez reçu cette alerte, Voici les étapes à suivre pour examiner:

1. Dans le message d’alerte, cliquez sur **afficher l’alerte** pour accéder à la page des **alertes** dans le centre de sécurité & conformité.

2. Sélectionnez l’alerte pour voir l’option permettant d' **afficher la liste des messages** ou d’afficher les **messages dans l’Explorateur**. Ces deux options vous permettent d’accéder aux détails du message, qui inclut l’ID du message. Notez que le lien de l’Explorateur de menaces filtre automatiquement les messages qui correspondent aux critères d’alerte. Vous devrez peut-être ajuster le filtre de date dans l’Explorateur de menaces.

Le message de hameçonnage a été remis en raison d’une substitution configurée manuellement:

- Un expéditeur ou domaine autorisé défini par l’utilisateur.

- Un expéditeur ou domaine autorisé défini par l’administrateur dans une stratégie de blocage du courrier indésirable.

- Une adresse IP autorisée dans une stratégie de filtrage des connexions.

- Une règle de flux de messagerie (également appelée règle de transport) qui est configurée pour autoriser les messages dans.

Si vous pensez que le message a été marqué de manière incorrecte comme hameçonnage, utilisez le [complément de message de rapport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook pour soumettre des exemples de messages à Microsoft.
