---
title: DLP de point de terminaison non déployé sur l’appareil de l’utilisateur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 2d5f0486ed8d4cbd95603f223bc0e48c4dcf38abb001d1616ca968b1d6bba7de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044230"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP de point de terminaison non déployé sur l’appareil de l’utilisateur

Si le paramètre de protection contre la perte de données (DLP) du point de terminaison ne s’est pas appliqué à l’appareil d’un utilisateur, vérifiez que vous répondez aux exigences suivantes :protection contre la perte de données :

- Windows 10 x64 build 1809 ou une version ultérieure est installé sur l'appareil.
- Le client anti-programme malveillant version 4.18.2009.7 ou version ultérieure est installé.
- L’appareil est **l’un** des suivants :
    
    - Jointure Azure Active Directory (Azure AD)
    - Jointure hybride Azure AD
    - Inscrit à AAD

- Pour appliquer des actions de stratégie, assurez-vous que le navigateur Microsoft Chromium Edge est installé sur l’appareil du point de terminaison.

Pour plus d’informations sur la configuration requise pour le déploiement de la protection contre la perte de données de point de terminaison, consultez [Prise en main la protection contre la perte de données de point de terminaison](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)