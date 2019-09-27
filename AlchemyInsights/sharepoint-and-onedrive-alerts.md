---
title: Ne pas recevoir d’alertes SharePoint et OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205521"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>Ne pas recevoir d’alertes SharePoint et OneDrive

Vérifiez d’abord le dossier courrier indésirable dans votre courrier électronique.

Déterminez ensuite si **toutes les alertes ne sont pas remises** ou si **une alerte individuelle** d’un fichier ou d’une bibliothèque spécifique n’est pas remise.

- Si **toutes les alertes provenant de plusieurs fichiers ou bibliothèques ne sont pas remises**, visitez le [tableau de bord état des services](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange. Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange. Notez également si d’autres e-mails sont remis (si ce n’est pas le cas), le problème est probablement lié à Exchange.
- Si **une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise**, essayez de la supprimer et de la recréer. Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) pour recréer l’alerte.

> [!NOTE]
> - Les alertes ne peuvent pas être envoyées à un groupe de distribution. Seuls les groupes Security et O365 sont pris en charge.
> - Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte. Vous devez utiliser le flux de travail Microsoft Flow ou SharePoint Designer pour y parvenir.
