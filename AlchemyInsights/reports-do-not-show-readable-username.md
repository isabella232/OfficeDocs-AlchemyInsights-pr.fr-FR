---
title: Les rapports du Centre d'administration Microsoft 365 n’indiquent pas le nom d’utilisateur de façon lisible
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "9008619"
ms.openlocfilehash: 63a412155c654e3a0d7913de3ec8222982017045
ms.sourcegitcommit: 744f03d1c3e6e22975fb96396686b112e385a82d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/02/2021
ms.locfileid: "58867029"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Les rapports du Centre d'administration Microsoft 365 n’indiquent pas le nom d’utilisateur de façon lisible

Les rapports du Centre d'administration Microsoft 365 n’indiquent pas les noms d’utilisateur, mais plutôt les valeurs numériques alpha, telles que B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ce comportement est attendu et a été communiqué dans le centre de messages (MC275344, publié le 3 août 2021). 

Les administrateurs globaux peuvent inverser cette modification pour leur client et afficher des informations utilisateur identifiables si les pratiques de confidentialité de leur organisation le permettent. Pour inverser la modification pour le client :

1. Dans le Centre d’administration, allez à **Paramètres** > **Paramètres de l’organisation** > **Services**, puis sélectionnez **Rapports**. 
1. Sous **Choisir comment afficher les informations utilisateur,** sélectionnez **Afficher les informations utilisateur identifiables dans les rapports**, ré-exécuter le rapport.