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
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757289"
---
# <a name="upgrade-azure-ad-connect"></a>Mettre à niveau Azure AD Connect

Par défaut, la mise à niveau automatique est activée pour Azure AD Connect, ce qui permet de s’assurer que vous utilisez la dernière version. Pour vérifier les paramètres de mise à niveau automatique, utilisez la cmdlet **Get-ADSyncAutoUpgrade** dans Azure ad PowerShell. L’applet de commande renvoie l’une des valeurs suivantes: 

- **Activé**: la mise à niveau automatique est activée.

- **Désactivé**: la mise à niveau automatique est désactivée.

- **Suspendu**: le système n’est plus autorisé à recevoir des mises à niveau automatiques. Vous ne pouvez pas configurer cette valeur; elle est définie par le système. 

Pour plus d’informations, consultez la rubrique [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pour télécharger la dernière version d’Azure AD Connect, accédez à [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
