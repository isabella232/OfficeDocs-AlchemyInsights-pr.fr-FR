---
title: Identifier le transfert de courrier électronique externe sur les boîtes aux lettres dans les journaux d’audit
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696295"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifier quand le transfert de courrier électronique externe est configuré sur les boîtes aux lettres

Lorsqu’un utilisateur de Microsoft 365 configure le transfert de messages externes sur une boîte aux lettres, l’activité est auditée dans le cadre de la cmdlet **Set-Mailbox** . Vous pouvez voir l’activité à l’aide de la recherche de journal d’audit dans le centre de sécurité & conformité.

1. Connectez-vous au [Centre de conformité & Microsoft 365 Security](https://protection.office.com/).

2. Accédez à la **Search**  >  page de**recherche du journal d’audit** de la recherche.

3. Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** . Vous n’avez pas besoin de spécifier un nom d’utilisateur. Vérifiez que le champ **activités** est défini sur **afficher les résultats pour toutes les activités**.

4. Cliquez sur **Rechercher**.

Dans les résultats, cliquez sur **Filtrer les résultats** et tapez **Set-Mailbox** dans la zone filtre d’activité. Sélectionnez un enregistrement d’audit dans les résultats. Dans la fenêtre mobile des **Détails** , cliquez sur **informations supplémentaires**. Vous devez examiner les détails de chaque enregistrement d’audit pour déterminer si l’activité est liée au transfert du courrier électronique.

- **ObjectID**: valeur d’alias de la boîte aux lettres qui a été modifiée.

- **Paramètres**: _ForwardingSmtpAddress_ indique l’adresse de messagerie cible.

- **Userid**: l’utilisateur qui a configuré le transfert du courrier électronique sur la boîte aux lettres dans le champ **ObjectID** .

Pour plus d’informations, consultez [la rubrique Détermination de la personne qui a configuré le transfert du courrier pour une boîte aux lettres](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
