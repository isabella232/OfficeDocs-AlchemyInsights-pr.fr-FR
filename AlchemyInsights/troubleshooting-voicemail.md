---
title: 'Résolution des problèmes de messagerie vocale '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: 36ba65c1ee67631a8b3c24c3407f46e3304541c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330742"
---
# <a name="troubleshooting-voicemail"></a>Résolution des problèmes de messagerie vocale

Assurez-vous que la fonctionnalité Busy on Busy est intentionnelle.

Si cette fonctionnalité n’est pas nécessaire pour cet utilisateur :

1. Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).
1. Sur le rail de gauche, **accédez aux stratégies**  >  **d’appel**  >  **vocal Gérer les stratégies** sur la stratégie **d’appel.**
1. Sélectionnez **Gérer les utilisateurs.**
1. Recherchez un utilisateur et modifiez la stratégie d’appel en une stratégie qui a Occupé sur le lieu de travail est **disponible lors d’un appel** à **l’autre.**
1. Cliquez sur **Appliquer**.

**Remarque**: la réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.

Pour plus d’informations sur cette fonctionnalité, voir : [Busy on Busy est disponible pendant un appel.](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)
