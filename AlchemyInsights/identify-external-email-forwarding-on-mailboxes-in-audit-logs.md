---
title: Identifier le transfert de courrier électronique externe sur les boîtes aux lettres dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539099"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifier quand le transfert de courrier électronique externe est configuré sur les boîtes aux lettres

Lorsqu’un utilisateur d’Office 365 configure le transfert de messages externes sur une boîte aux lettres, l’activité est auditée dans le cadre de la cmdlet **Set-Mailbox** . Vous pouvez voir l’activité à l’aide de la recherche de journal d’audit dans le centre de sécurité & conformité.

1. Connectez-vous au [Centre de sécurité & conformité Office 365](https://protection.office.com/).

2. Accédez à la page de**recherche du journal d’audit** de la **recherche** > .

3. Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** . Vous n’avez pas besoin de spécifier un nom d’utilisateur. Vérifiez que le champ **activités** est défini sur **afficher les résultats pour toutes les activités**.

4. Cliquez sur **Rechercher**.

Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone filtre d’activité. Sélectionnez un enregistrement d’audit dans les résultats. Dans la fenêtre mobile des **Détails** , cliquez sur **informations supplémentaires**. Vous devez examiner les détails de chaque enregistrement d’audit pour déterminer si l’activité est liée au transfert du courrier électronique.

- **ObjectID**: valeur d’alias de la boîte aux lettres qui a été modifiée.

- **Paramètres**: _ForwardingSmtpAddress_ indique l’adresse de messagerie cible.

- **Userid**: l’utilisateur qui a configuré le transfert du courrier électronique sur la boîte aux lettres dans le champ **ObjectID** .

Pour plus d’informations, consultez [la rubrique Détermination de la personne qui a configuré le transfert du courrier pour une boîte aux lettres](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
