---
title: Rechercher l’adresse IP dans le journal d’audit
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902258"
---
# <a name="find-the-ip-address-in-audit-log"></a>Rechercher l’adresse IP dans le journal d’audit

L’adresse IP qui correspond à une activité effectuée par un utilisateur ou un administrateur est affichée dans les journaux d’audit. Les informations client sont également enregistrées. Voici comment identifier l’adresse IP :

1. Faites l’une des actions suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Si vous voyez une notification vous avisant que vous devez activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas activée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.

2. Dans la page **Audit,** vérifiez que **l’onglet** Recherche est sélectionné, puis configurez les paramètres suivants :
   - **Date et plage de dates :** sélectionnez la plage date/heure dans les zones Début **et** Fin. 
   - **Activités :** si vous êtes intéressé par une activité spécifique, sélectionnez-la dans la liste ; Sinon, la valeur par défaut **Afficher les résultats pour toutes les activités** renvoie toutes les activités qui seront renvoyées. Notez que certaines activités peuvent ne pas être disponibles pour la sélection ; toutefois, ces éléments d’audit sont renvoyés si **afficher les résultats de toutes les** activités est sélectionné.
   - **Utilisateurs**: acceptez la valeur par défaut vide pour renvoyer des résultats pour tous les utilisateurs, ou entrez un ou plusieurs utilisateurs.

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.**

4. Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone de filtrage des activités.

5. Sélectionnez un enregistrement d’audit dans les résultats pour ouvrir le volant **Détails.**

Pour plus d’informations, [consultez la recherche dans le journal d’audit pour examiner les problèmes de support courants.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
