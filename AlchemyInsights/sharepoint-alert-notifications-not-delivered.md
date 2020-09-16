---
title: Notifications d’alerte SharePoint non remises
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751241"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Notifications d’alerte SharePoint non remises

Vérifiez le dossier de courrier indésirable dans votre courrier électronique, car des alertes pourraient y figurer.

Déterminez si **toutes les alertes ne sont pas remises** ou si **une alerte individuelle** d’un fichier ou d’une bibliothèque spécifique n’est pas remise.

- **Les alertes individuelles ne sont pas remises**: si une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise, vous pouvez essayer de la supprimer et de la recréer. Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) pour recréer l’alerte.
- **Toutes les alertes ne sont pas remises**: si toutes les alertes provenant de plusieurs fichiers ou bibliothèques ne sont pas remises, consultez le [tableau de bord État du service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange. Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange. Il est également important de noter si d’autres e-mails sont remis et, si ce n’est pas le cas, le problème est probablement lié à Exchange.

FAQ sur les alertes :

- Il n’est pas possible d’envoyer des alertes à un groupe de distribution, seuls les groupes Security et O365 sont pris en charge.
- Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte ; vous devez utiliser le flux de travail Microsoft FLOW ou SharePoint Designer pour y parvenir.

## <a name="related-topics"></a>Voir aussi

Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?

- [Créer un flux](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint et flux](https://flow.microsoft.com//blog/sharepoint-and-flow/)
