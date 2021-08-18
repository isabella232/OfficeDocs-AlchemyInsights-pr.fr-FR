---
title: Identifier le forwarding de courrier externe sur les boîtes aux lettres dans les journaux d’audit
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899882"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifier le moment où le forwarding de courrier externe est configuré sur les boîtes aux lettres

Lorsqu’un Microsoft 365 configure le forwarding de courrier externe sur une boîte aux lettres, l’activité est auditée dans le cadre de la cmdlet **Set-Mailbox.** Vous pouvez voir l’activité à l’aide de la recherche dans le journal d’audit. Voici comment faire.

1. Effectuez l’une des étapes suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Solutions** \> **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://compliance.microsoft.com/auditlogsearch> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Audit**. Ou, pour aller directement à la page **Audit,** utilisez <https://sip.security.microsoft.com/auditlogsearch> .

2. Dans la page **Audit,** vérifiez que **l’onglet** Recherche est sélectionné, puis configurez les paramètres suivants :
   - Sélectionnez la plage date/heure dans les zones **Début** **et** Fin.
   - Vérifiez que **la zone Activités** contient Afficher les résultats pour toutes les **activités.**

3. Lorsque vous avez terminé, cliquez sur **Rechercher.** Les activités apparaissent sur la nouvelle page **de recherche d’audit.**

4. Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone de filtrage des activités.

5. Sélectionnez un enregistrement d’audit dans les résultats. Dans le **volant Détails,** cliquez sur **Plus d’informations.** Vous devez examiner les détails de chaque enregistrement d’audit pour déterminer si l’activité est liée au forwarding de courrier électronique.

   - **ObjectId**: valeur d’alias de la boîte aux lettres modifiée.
   - **Paramètres**: _ForwardingSmtpAddress_ indique l’adresse de messagerie cible.
   - **UserId :** utilisateur qui a configuré le forwarding de courrier sur la boîte aux lettres dans le **champ ObjectId.**

Pour plus d’informations, voir Déterminer qui [a installé le forwarding de courrier pour une boîte aux lettres.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
