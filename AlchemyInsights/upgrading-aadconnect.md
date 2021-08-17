---
title: 932 Mise à niveau d’AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104810"
---
# <a name="upgrade-azure-ad-connect"></a>Mettre à niveau les Connecter Azure AD

Par défaut, la mise à niveau automatique est activée pour les Connecter Azure AD, ce qui permet de s’assurer que vous exécutez la dernière version. Pour vérifier les paramètres de mise à niveau automatique, utilisez l’cmdlet **Get-ADSyncAutoUpgrade** dans Azure AD PowerShell. L’cmdlet retourne l’une des valeurs suivantes :

- **Activé :** la mise à niveau automatique est activée.

- **Désactivé :** la mise à niveau automatique est désactivée.

- **Suspendu :** le système n’est plus éligible pour recevoir des mises à niveau automatiques. Vous ne pouvez pas configurer cette valeur ; Elle est définie par le système.

Pour plus d’informations, voir [Mise à niveau automatique.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Pour télécharger la dernière version d’Azure AD Connecter, allez sur [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
