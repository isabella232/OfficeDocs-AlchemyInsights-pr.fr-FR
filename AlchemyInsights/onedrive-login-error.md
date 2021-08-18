---
title: OneDrive de connexion AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112910"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive de connexion AADSTS50011

Si vous recevez une erreur « AADSTS50011 : l’URL de réponse spécifiée dans la demande ne correspond pas à la réponse » lors de la signature de l’application OneDrive, recherchez les données suivantes :

Votre OneDrive version doit être égale ou supérieure à la version 20.052.XXXX.XXXX. Pour vérifier votre version, cliquez sur l’icône OneDrive bleu dans la zone de notification, sélectionnez Aide **& Paramètres > Paramètres > à propos de**.

Votre réseau peut bloquer le trafic **vers g.live.com** et **oneclient.sfx.ms**. Si ce trafic est bloqué, OneDrive ne peut pas se mettre à jour lui-même. Travaillez avec votre administrateur réseau pour vous assurer que vous avez accès à ces URL. [Ces points de terminaison doivent](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) être accessibles aux clients qui utilisent Microsoft 365 plans.

Si vous devez obtenir manuellement une version actuelle de OneDrive, visitez [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
