---
title: Les rapports dans Centre d'administration Microsoft 365 n’indiquent pas le nom d’utilisateur lisible
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
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327812"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Les rapports dans Centre d'administration Microsoft 365 n’indiquent pas le nom d’utilisateur lisible

Les rapports dans Centre d'administration Microsoft 365 n’indiquent pas les noms d’utilisateur, mais plutôt les valeurs numériques alpha, telles que B2BC6C15BB9FCDEA71E5CD302D228CC8.

This is expected behavior and has been communicated in the Message Center (MC275344, published Aug. 3, 2021). 

Les administrateurs globaux peuvent revenir sur cette modification pour leur locataire et afficher les informations identifiables de l'utilisateur si les pratiques de confidentialité de leur organisation le permettent. Pour annuler la modification pour le locataire :

1. Dans le Centre d’administration, **Paramètres** Services de  >  **paramètres** d’organisation,  >  [](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )puis sélectionnez **Rapports.** 
1. Sous **Choisir comment afficher les informations utilisateur,** sélectionnez Afficher les informations utilisateur identifiables dans les **rapports,** puis ré-exécuter le rapport.