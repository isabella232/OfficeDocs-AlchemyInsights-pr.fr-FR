---
title: Erreur de fermeture de la connexion sous-jacente dans SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 1b4f336f389eb6fd81ac2ca40e6047184cc4c1bf
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317694"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Erreur « La connexion sous-jacente a été fermée » dans SharePoint

Si vous recevez l’erreur « La connexion sous-jacente a été fermée » dans SharePoint, cela peut être lié au retrait de TLS 1.0/1.1. Pour plus d’informations, consultez ces articles :

- [Préparation de TLS 1.2 dans Office 365 et Office 365 Cloud de la communauté du secteur public](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Des erreurs d’authentification se produisent si le client n’a pas de prise en charge TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Mise à jour pour activer TLS 1.1 et TLS 1.2 comme protocoles sécurisés par défaut dans WinHTTP sous Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Si des utilisateurs utilisent Windows 7, assurez-vous qu’ils vérifient les [Suites de chiffrement TLS dans Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).