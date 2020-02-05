---
title: Retarde la réception des alertes OneDrive et SharePoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771213"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Retarde la réception des alertes OneDrive et SharePoint

- Vérifiez d’abord le dossier courrier indésirable dans votre courrier électronique.
- Si **toutes les alertes provenant de plusieurs fichiers ou bibliothèques sont retardées**, visitez le [tableau de bord État du service](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange. Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange. Notez également si d’autres e-mails sont remis (si ce n’est pas le cas), le problème est probablement lié à Exchange.
- Si **une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise**, essayez de la supprimer et de la recréer. Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) pour recréer l’alerte.

> [!NOTE]
> - Les alertes ne peuvent pas être envoyées à un groupe de distribution. Seuls les groupes Security et O365 sont pris en charge.
> - Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte. Vous devez utiliser le flux de travail Microsoft Flow ou SharePoint Designer pour y parvenir.
