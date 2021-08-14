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
ms.openlocfilehash: e639d74cd8dbbb03ffb5b253451c99c8fe639f024a46e173845a0f4d322e43ca
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972381"
---
# <a name="troubleshooting-voicemail"></a>Résolution des problèmes de messagerie vocale

Assurez-vous que la fonctionnalité Busy on Busy est intentionnelle.

Si cette fonctionnalité n’est pas nécessaire pour cet utilisateur :

1. Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).
1. Sur le rail de gauche, **accédez aux stratégies**  >  **d’appel**  >  **vocal Gérer les stratégies** sur la stratégie **d’appel.**
1. Sélectionnez **Gérer les utilisateurs.**
1. Recherchez un utilisateur et modifiez la stratégie d’appel en une stratégie qui a Occupé sur le lieu de travail est **disponible lors d’un appel** à **l’autre.**
1. Cliquez sur **Appliquer**.
> [!NOTE]
> La réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.

Pour plus d’informations sur cette fonctionnalité, voir : [Busy on Busy est disponible pendant un appel.](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)
