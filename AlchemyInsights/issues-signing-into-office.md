---
title: Problèmes de la signature à Microsoft 365 applications
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744634"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problèmes de la signature Microsoft 365 Apps

Remarque : si vous utilisez une version antérieure de Windows (par exemple, Windows 7 SP1, Windows Server 2008 R2), utilisez le correctif simple pour activer TLS 1.2 par défaut. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Pour plus d’informations, consultez [Mise à jour pour activer TLS 1.1 et TLS 1.2 comme protocoles sécurisés par défaut dans WinHTTP dans Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Pour résoudre les problèmes de connexion avec les applications Microsoft 365, essayez les options suivantes sur l’ordinateur concerné :  

- Pour plus Windows, voir Recommandations sur la résolution des problèmes [courants de sign-in](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Pour Mac, voir [Can’t sign in to an Office 2016 pour Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Conseil** sur les ordinateurs Windows, nous pouvons diagnostiquer et résoudre automatiquement pour vous plusieurs problèmes courants liés à la connexion à Office. Téléchargez et exécutez **[L’Assistant Support et Récupération de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** pour utiliser notre outil automatisé.

**Remarque :** La désactivation de l’authentification moderne (ADAL) ou de la gestion des comptes Web (WAM) pour résoudre les problèmes de la signature ou de l’activation **n’est pas recommandée.** Si les erreurs se produisent lors de la connexion à Microsoft 365 à [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) l’aide de Office 2013, veillez à activer l’authentification moderne pour Office client.

Pour des actions de dépannage spécifiques, voir :

[Problèmes de connexion lors de l’ouverture de session après la mise à jour vers Office 2016 build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Vous ne pouvez pas vous inscrire à votre compte d’organisation comme Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Comment résoudre les problèmes des applications non-navigateur qui ne peuvent pas se Office 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Invité à plusieurs reprises à obtenir des informations d’identification dans Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)