---
title: Examiner toutes les activités des utilisateurs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332341"
---
# <a name="investigate-all-the-users-activities"></a>Examiner toutes les activités des utilisateurs

Voici comment faire :

1. Faites l’une des actions suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://security.microsoft.com/auditlogsearch> .

    **Remarque**: si vous voyez une notification vous avisant que vous devez activer la fonctionnalité, allez de l’avant et l’activer maintenant. Si la fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.

2. Sous **l’onglet** Recherche de la page **Audit,** configurez les paramètres suivants :
   - **Date et plage de dates :** sélectionnez la plage date/heure dans les zones Début **et** Fin. 
   - **Activités :** si vous êtes intéressé par une activité spécifique, sélectionnez-la dans la liste ; Sinon, la valeur par défaut **Afficher les résultats pour toutes les activités** renvoie toutes les activités.
   - **Utilisateurs**: acceptez la valeur par défaut vide pour renvoyer des résultats pour tous les utilisateurs, ou entrez un ou plusieurs utilisateurs.

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.** Vous verrez l’adresse **IP,** **l’utilisateur** et le nom **de l’activité.**

4. Pour télécharger les résultats, **sélectionnez Exporter** \> **télécharger tous les résultats.**

5. Sélectionnez une activité dans les résultats pour ouvrir le volant de détails.

Pour en savoir plus, [consultez la recherche dans le journal d’audit pour examiner les problèmes de support courants.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
