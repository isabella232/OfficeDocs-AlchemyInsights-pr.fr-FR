---
title: Notifications d’alerte SharePoint non remises
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 978ca8df40736228932ae6f6a7c33ad0b159d4e5
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40047065"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Notifications d’alerte SharePoint non remises

Vérifiez le dossier de courrier indésirable dans votre courrier électronique, car des alertes pourraient y figurer.

Déterminez si **toutes les alertes ne sont pas remises** ou si **une alerte individuelle** d’un fichier ou d’une bibliothèque spécifique n’est pas remise.

- **Les alertes individuelles ne sont pas remises**: si une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise, vous pouvez essayer de la supprimer et de la recréer. Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) pour recréer l’alerte.
- **Toutes les alertes ne sont pas remises**: si toutes les alertes provenant de plusieurs fichiers ou bibliothèques ne sont pas remises, consultez le [tableau de bord État du service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange. Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange. Il est également important de noter si d’autres e-mails sont remis et, si ce n’est pas le cas, le problème est probablement lié à Exchange.

FAQ sur les alertes :

- Il n’est pas possible d’envoyer des alertes à un groupe de distribution, seuls les groupes Security et O365 sont pris en charge.
- Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte ; vous devez utiliser le flux de travail Microsoft FLOW ou SharePoint Designer pour y parvenir.

Informations supplémentaires :

- **Configuration**des alertes : pour plus d’informations sur la configuration des alertes, consultez [la rubrique créer une alerte pour être averti lorsqu’un fichier ou un dossier est modifié dans SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Dépannage des alertes**: pour plus d’informations sur la résolution des alertes, consultez la rubrique [les utilisateurs ne reçoivent pas les notifications d’alerte SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Stratégies avancées d’alerte de conformité O365**: pour plus d’informations sur la configuration de ces alertes, consultez [la rubrique stratégies d’alerte de conformité](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **Journaux d’audit SharePoint et OneDrive**: pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Alertes envoyées par protection avancée contre les menaces**: consultez la rubrique [ATP pour SharePoint et OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Alertes envoyées par les stratégies de protection contre la perte de données**: consultez la rubrique [notifications par courrier électronique pour les stratégies DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Rubriques connexes

Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?

- [Créer un flux](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint et flux](https://flow.microsoft.com//blog/sharepoint-and-flow/)
