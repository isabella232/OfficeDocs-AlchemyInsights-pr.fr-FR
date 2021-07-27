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
ms.openlocfilehash: c3a0695dc2aa5f6e56be2235f08c81dbbe7fcea2
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532916"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitations des étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive

Lorsque vous activez des étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive, tenez compte des exigences et des limitations, notamment :

- SharePoint et OneDrive ne peuvent pas traiter certains fichiers étiquetés et chiffrés à partir d’applications de bureau Office lorsque les fichiers contiennent des données PowerQuery, des données stockées par des compléments personnalisés ou des parties XML personnalisées.
- SharePoint et OneDrive n’appliquent pas automatiquement les étiquettes de confidentialité aux fichiers existants que vous avez déjà chiffrés à l’aide d’étiquettes Azure Information Protection (AIP). Pour appliquer des étiquettes de confidentialité aux fichiers chiffrés : 
    - Assurez-vous que les étiquettes AIP ont été migrées et publiées dans le Centre de conformité Microsoft 365.
    - Téléchargez les fichiers étiquetés, puis chargez-les à leur emplacement SharePoint ou OneDrive d’origine.
- Pour les documents chiffrés, l’impression n’est pas prise en charge.

Pour plus d’informations sur les limitations, consultez [Activer les étiquettes de confidentialité pour les fichiers Office dans SharePoint et OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
