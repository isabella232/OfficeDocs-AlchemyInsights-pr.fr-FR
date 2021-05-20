---
title: Simulateur d’attaques 2681 dans Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545724"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulateur d’attaques dans Microsoft 365

- Le Simulateur d’attaques vous manque ? Le Simulateur d’attaques **nécessite Microsoft Defender Office 365 plan 2** ou Office 365 Entreprise **E5.** Le Simulateur  d’attaques n’est pas inclus dans Microsoft Defender pour Office 365 Plan 1, Office 365 Entreprise E3 ou les abonnements Applications Microsoft 365 pour les PME de service.

- Le compte que vous utilisez pour lancer des attaques simulées nécessite des autorisations d’administrateur général ou d’administrateur de sécurité et une authentification multifacteur (MFA). Pour plus d’informations sur les exigences du simulateur d’attaques, [consultez cette rubrique.](/microsoft-365/security/office-365-security/attack-simulator)

- Points importants à connaître sur les simulations d’attaques **par mot** de passe en force brute :

  - Si l’authentification multifacteur est activée sur le compte cible et que le mot de passe a été deviné correctement, le compte ne sera pas compromis (le deuxième facteur d’authentification sera incomplet).

  - Le fichier de mot de passe ne peut pas être supérieur à 10 Mo. Utilisez un mot de passe par ligne et incluez une ligne vide (retour chariot) après le dernier mot de passe de la liste.

- Points importants à connaître sur les simulations d’attachement de **harponnage** :

  - Par conception, vous ne pouvez pas fournir de valeur personnalisée pour l’URL du serveur de connexion au **hameçonnage.**

  - Si un destinataire utilise le [add-in Activer](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) le message de rapport pour signaler le message comme hameçonnage, il se peut que vous ne receviez pas d’alertes pour le message (car il s’agit d’une attaque simulée).

- Rapports : une fois l’attaque simulée terminée, vous pouvez cliquer sur **Détails** de l’attaque pour voir le rapport.

- Pour obtenir des instructions détaillées et de nouvelles fonctionnalités dans le Simulateur d’attaques, voir Simulateur [d’attaques dans Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
