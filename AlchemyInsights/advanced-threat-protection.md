---
title: Microsoft Defender pour Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: 61236d1e0174248cdb49284d6c6c7d49df51e7e9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315076"
---
# <a name="microsoft-defender-for-office-365"></a>Microsoft Defender pour Office 365

- Coffre Les pièces jointes, Coffre liens et l’anti-hameçonnage font partie de Microsoft Defender pour Office 365. Enterprise E5, Éducation A5 et Microsoft 365 Business Premium inclure Microsoft Defender pour Office 365. Tous les autres plans nécessitent un module de développement Microsoft Defender pour Office 365 abonnement.

- Vous devez attribuer les licences appropriées pour protéger vos utilisateurs par Microsoft Defender Office 365. Voir [Ajouter des utilisateurs et attribuer des licences](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) en même temps pour obtenir des instructions sur la façon d’appliquer des licences en bloc à vos utilisateurs.

- Les administrateurs globaux ou les administrateurs de sécurité peuvent accéder aux fonctionnalités de Microsoft Defender pour Office 365 dans le portail Microsoft 365 Defender dans la section Collaboration sur la messagerie **&** Stratégies & règles de menace \>  \> .

- Coffre Les pièces jointes et Coffre de liens peuvent être limitées à des domaines, des membres de groupe ou des utilisateurs individuels spécifiques. Vous pouvez également spécifier des exceptions pour Coffre pièces jointes et Coffre de liens en fonction du domaine, de l’appartenance à un groupe ou des utilisateurs individuels.

- Il n’existe aucune stratégie Coffre pièces jointes par défaut qui protège les messages électroniques. Vous devez créer [une stratégie pour la protection Coffre](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-attachments-policies) pièces jointes dans le courrier électronique.

  Coffre Les pièces jointes SharePoint, OneDrive et Microsoft Teams sont activées ou désactivées globalement et ne nécessitent pas Coffre stratégies de pièces jointes. Pour plus d’informations, [voir Coffre attachments for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/mdo-for-spo-odb-and-teams).

- Il n’existe aucune stratégie Coffre liens par défaut qui protège les messages électroniques ou les Microsoft Teams. Vous devez créer [une stratégie pour la](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies) protection Coffre liens dans les e-mails et Teams.

  Coffre La protection des liens pour les applications Office 365 est appliquée à tous les utilisateurs de l’organisation qui sont titulaires d’une licence Defender pour Office 365, que les utilisateurs soient inclus ou non dans les stratégies de liens Coffre actives. Pour plus d’informations, [Coffre paramètres de liens](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links#safe-links-settings-for-office-365-apps)pour Office 365 applications.
