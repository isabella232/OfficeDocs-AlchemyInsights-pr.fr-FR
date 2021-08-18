---
title: Récupérer les journaux d’audit
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: ac2e5eafbb92b234697c22f73cd565af9d7c3508
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329492"
---
# <a name="retrieve-the-audit-logs"></a>Récupérer les journaux d’audit

Lorsque vous ouvrez le journal d’audit pour la première fois, il est vide. Vous devez effectuer une recherche pour afficher le contenu. Voici comment effectuer une recherche générale de toutes les activités :

1. Effectuez l’une des étapes suivantes :
   - Dans le Centre de conformité Microsoft 365 à <https://compliance.microsoft.com>, accédez à **Solutions**\>**Audit**. Ou, pour accéder directement à la page **Audit**, utilisez <https://compliance.microsoft.com/auditlogsearch>.
   - Dans le Portail Microsoft 365 Defender à <https://security.microsoft.com>, accédez à **Audit**. Ou, pour accéder directement à la page **Audit**, utilisez <https://sip.security.microsoft.com/auditlogsearch>.

2. Dans la page **Audit**, vérifiez que l’onglet **recherche** est sélectionné, puis configurez les paramètres suivants :
   - **Plage de dates et d’heures** : sélectionnez la plage de date/heure dans les zones **Début** et **Fin**.
   - **Activités** : vérifiez que **Afficher les résultats de toutes les activités** est sélectionné.
   - **Utilisateurs** : acceptez la valeur par défaut vide pour renvoyer des résultats pour tous les utilisateurs, ou entrez un ou plusieurs utilisateurs.

3. Lorsque vous avez terminé, cliquez sur **Rechercher**. Les activités apparaissent sur la nouvelle page **Recherche d’audit**.

4. Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone de filtre d’activité.

5. Sélectionnez un enregistrement d’audit dans les résultats. Dans le menu volant **Détails**, cliquez sur **Plus d’informations** pour afficher d’autres d’informations telles que client, utilisateur ayant effectué une action, etc.
