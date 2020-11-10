---
title: Erreur de connexion OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947486"
---
# <a name="onedrive-login-error-aadsts50011"></a>Erreur de connexion OneDrive AADSTS50011

Si vous recevez une erreur « AADSTS50011 : l’URL de réponse spécifiée dans la demande ne correspond pas à la réponse » lorsque vous vous connectez à l’application OneDrive, vérifiez les points suivants :

Votre version de OneDrive doit être supérieure ou égale à la version 20.052. XXXX. XX. Pour vérifier votre version, cliquez sur l’icône OneDrive en bleu dans la zone de notification, sélectionnez **aide & paramètres > paramètres > à propos** de.

Votre réseau peut bloquer le trafic vers **g.live.com** et **oneclient.SFX.ms**. Si ce trafic est bloqué, OneDrive ne peut pas se mettre à jour lui-même. Collaborez avec votre administrateur réseau pour vous assurer que vous avez accès à ces URL. [Ces points de terminaison](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) doivent être accessibles aux clients qui utilisent des plans Microsoft 365.

Si vous avez besoin d’obtenir manuellement une version actuelle de OneDrive, visitez [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
