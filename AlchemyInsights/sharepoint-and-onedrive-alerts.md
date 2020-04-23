---
title: Retarde la réception des alertes OneDrive et SharePoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741999"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Retarde la réception des alertes OneDrive et SharePoint

- Vérifiez d’abord le dossier courrier indésirable dans votre courrier électronique.
- Si **toutes les alertes provenant de plusieurs fichiers ou bibliothèques sont retardées**, visitez le [tableau de bord État du service](https://portal.office.com/adminportal/home?ref=/servicehealth) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange. Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange. Notez également si d’autres e-mails sont remis (si ce n’est pas le cas), le problème est probablement lié à Exchange.
- Si **une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise**, essayez de la supprimer et de la recréer. Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) pour recréer l’alerte.

> [!NOTE]
> - Les alertes ne peuvent pas être envoyées à un groupe de distribution. Seuls les groupes Security et O365 sont pris en charge.
> - Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte. Vous devez utiliser le flux de travail Microsoft Flow ou SharePoint Designer pour y parvenir.
