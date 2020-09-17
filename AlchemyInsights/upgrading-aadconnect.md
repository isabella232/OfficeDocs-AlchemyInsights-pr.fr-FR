---
title: 932 mise à niveau de AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806037"
---
# <a name="upgrade-azure-ad-connect"></a>Mettre à niveau Azure AD Connect

Par défaut, la mise à niveau automatique est activée pour Azure AD Connect, ce qui permet de s’assurer que vous utilisez la dernière version. Pour vérifier les paramètres de mise à niveau automatique, utilisez la cmdlet **Get-ADSyncAutoUpgrade** dans Azure ad PowerShell. L’applet de commande renvoie l’une des valeurs suivantes :

- **Activé**: la mise à niveau automatique est activée.

- **Désactivé**: la mise à niveau automatique est désactivée.

- **Suspendu**: le système n’est plus autorisé à recevoir des mises à niveau automatiques. Vous ne pouvez pas configurer cette valeur ; elle est définie par le système.

Pour plus d’informations, consultez la rubrique [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pour télécharger la dernière version d’Azure AD Connect, accédez à [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
