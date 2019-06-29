---
title: 932 mise à niveau de AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365893"
---
# <a name="upgrade-azure-ad-connect"></a>Mettre à niveau Azure AD Connect

Par défaut, la mise à niveau automatique est activée pour Azure AD Connect, ce qui permet de s’assurer que vous utilisez la dernière version. Pour vérifier les paramètres de mise à niveau automatique, utilisez la cmdlet **Get-ADSyncAutoUpgrade** dans Azure ad PowerShell. L’applet de commande renvoie l’une des valeurs suivantes:

- **Activé**: la mise à niveau automatique est activée.

- **Désactivé**: la mise à niveau automatique est désactivée.

- **Suspendu**: le système n’est plus autorisé à recevoir des mises à niveau automatiques. Vous ne pouvez pas configurer cette valeur; elle est définie par le système.

Pour plus d’informations, consultez la rubrique [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pour télécharger la dernière version d’Azure AD Connect, accédez à [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
