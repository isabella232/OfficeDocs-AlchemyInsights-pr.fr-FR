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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630247"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifier le moment où le forwarding de courrier externe est configuré sur les boîtes aux lettres

Lorsqu’un Microsoft 365 configure le forwarding de courrier externe sur une boîte aux lettres, l’activité est auditée dans le cadre de la cmdlet **Set-Mailbox.** Vous pouvez voir l’activité à l’aide de la recherche dans le journal d’audit dans le Centre de sécurité & conformité.

1. Connectez-vous au [Centre Microsoft 365 conformité.](https://protection.office.com/)

2. Go to the **Search**  >  **Audit log search** page.

3. Sélectionnez la plage de dates dans les champs **Date de** début et **Date de** fin. Vous n’avez pas besoin de spécifier un nom d’utilisateur. Vérifiez que **le champ Activités** est définie pour afficher les résultats de toutes les **activités.**

4. Cliquez sur **Rechercher**.

Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone de filtrage des activités. Sélectionnez un enregistrement d’audit dans les résultats. Dans le **volant Détails,** cliquez sur **Plus d’informations.** Vous devez examiner les détails de chaque enregistrement d’audit pour déterminer si l’activité est liée au forwarding du courrier électronique.

- **ObjectId**: valeur d’alias de la boîte aux lettres modifiée.

- **Paramètres**: _ForwardingSmtpAddress_ indique l’adresse de messagerie cible.

- **UserId :** utilisateur qui a configuré le forwarding de courrier sur la boîte aux lettres dans le **champ ObjectId.**

Pour plus d’informations, voir Déterminer qui a installé le forwarding de courrier [pour une boîte aux lettres.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
