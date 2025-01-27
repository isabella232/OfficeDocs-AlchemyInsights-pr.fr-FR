---
title: Limitations des étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: 376c0293c325a725c117d54bb0f15b0146b9224c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332815"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitations des étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive

Lorsque vous activez des étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive, tenez compte des exigences et des limitations, notamment :

- SharePoint et OneDrive ne peuvent pas traiter certains fichiers étiquetés et chiffrés à partir d’applications de bureau Office lorsque les fichiers contiennent des données PowerQuery, des données stockées par des compléments personnalisés ou des parties XML personnalisées.
- SharePoint et OneDrive n’appliquent pas automatiquement les étiquettes de confidentialité aux fichiers existants que vous avez déjà chiffrés à l’aide d’étiquettes Azure Information Protection (API). Pour appliquer des étiquettes de sensibilité aux fichiers cryptés : 
    - Assurez-vous que les étiquettes AIP ont été migrées et publiées dans le Centre de conformité Microsoft 365.
    - Téléchargez les fichiers étiquetés, puis chargez-les à leur emplacement SharePoint ou OneDrive d’origine.
- Pour les documents chiffrés, l’impression n’est pas prise en charge.

Pour plus d’informations sur les limitations, consultez [Activer les étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
