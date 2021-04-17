---
title: "Problème d'activation/de sign-in : le module de plateforme de confiance a mal fonctionne"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822885"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Résolution du message des applications Microsoft 365 « Le module de plateforme de confiance de votre ordinateur ne fonctionne pas correctement »

Pour corriger cette erreur, procédez comme suit :

1. Ouvrez une application Office, puis [se déconnecter](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de tous les comptes d’utilisateur existants.   
2. À **l'aide des comptes**  >  **de paramètres**  >  **Windows, & comptes** de messagerie, supprimez les comptes de travail existants. 
3. À l'aide **de** Windows  >  **Settings Accounts**  >  **Access work or school,** déconnectez les comptes existants. 
4. Réactiver l’état d’activation de Microsoft Office. [Découvrir comment](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Essayez le processus [de récupération utilisateur pour](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) corriger les défaillances du module de plateforme de confiance (TPM).