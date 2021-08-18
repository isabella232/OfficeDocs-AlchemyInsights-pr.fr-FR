---
title: Savoir qui a installé le forwarding sur une boîte aux lettres et comment
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317806"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Savoir qui a installé le forwarding sur une boîte aux lettres et comment

Si le forwarding externe a été définie sur une boîte aux lettres, l’activité est auditée dans le cadre de la cmdlet **Set-Mailbox.** Voici comment rechercher l’activité dans le journal d’audit :

1. Faites l’une des actions suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://security.microsoft.com/auditlogsearch> .

   **Remarque**: si vous voyez une notification vous avisant que vous devez activer l’audit, allez de l’avant et l’activer maintenant. Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.

2. Dans la page **Audit,** vérifiez que **l’onglet** Recherche est sélectionné, puis configurez les paramètres suivants :
   - Sélectionnez la plage date/heure dans les zones **Début** **et** Fin.
   - Vérifiez que **la zone Activités** contient Afficher les résultats pour toutes les **activités.**

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.**

4. Dans les résultats, cliquez sur la colonne **Activité** pour trier les résultats et recherchez les entrées **Set-Mailbox.**

5. Sélectionnez une activité dans les résultats pour ouvrir le volant de détails. Vous devez examiner les détails de chaque enregistrement d’audit pour déterminer si l’activité est liée au forwarding de courrier électronique :
   - **ObjectId**: valeur d’alias de la boîte aux lettres modifiée.
   - **Paramètres**: _ForwardingSmtpAddress_ indique l’adresse de messagerie cible.
   - **UserId :** utilisateur qui a configuré le forwarding de courrier sur la boîte aux lettres dans le **champ ObjectId.**

Pour plus d’informations, voir Déterminer qui a installé le forwarding de courrier [pour une boîte aux lettres.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
