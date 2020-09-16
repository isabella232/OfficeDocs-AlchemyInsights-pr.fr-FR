---
title: 2681 simulateur d’attaque dans Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759217"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulateur d’attaque dans Microsoft 365

- Vous ne disposez pas d’un simulateur d’attaque ? Le simulateur d’attaque nécessite **office 365 Advanced Threat Protection Plan 2 (ATP plan 2)** ou **Office 365 entreprise E5**. Le simulateur d’attaque n’est **pas** inclus dans Office 365 Advanced Threat Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3 ou tout abonnement aux applications Microsoft 365 apps pour les entreprises.

- Le compte que vous utilisez pour lancer des attaques simulées requiert des autorisations d’administrateur général ou d’administrateur de sécurité, ainsi qu’une authentification multifacteur (MFA). Pour plus d’informations sur les exigences en matière de simulateur d’attaque, consultez [cette rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Éléments importants à connaître sur les simulations d’attaques **de mot de passe** en force :

  - Si l’authentification multifacteur est activée pour le compte cible et que le mot de passe a été deviné correctement, le compte ne s’affichera pas comme compromis (le deuxième facteur d’authentification sera incomplet).

  - Le fichier de mot de passe ne peut pas être supérieur à 10 Mo. Utilisez un mot de passe par ligne et incluez une ligne vide (retour chariot) après le dernier mot de passe de la liste.

- Éléments importants à connaître sur les simulations d’attachement de **Spear Phishing** :

  - Par défaut, vous ne pouvez pas fournir de valeur personnalisée pour l' **URL du serveur de connexion d’hameçonnage**.

  - Si un destinataire utilise le [complément activer le message de rapport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pour signaler le message comme hameçonnage, il se peut que vous ne receviez pas d’alertes pour le message (car il s’agit d’une attaque simulée).

- Rapports : une fois l’attaque simulée terminée, vous pouvez cliquer sur détails de l' **attaque** pour afficher le rapport.

- Pour obtenir des instructions détaillées et de nouvelles fonctionnalités dans le simulateur d’attaque, consultez la rubrique [attaques de simulateur dans Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
