---
title: Problèmes liés à SharePoint sur les ordinateurs Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066991"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problèmes liés à SharePoint sur les ordinateurs Windows 7

Si vous recevez des erreurs sur les ordinateurs Windows 7 lorsque vous travaillez sur SharePoint ou OneDrive, ils pourraient être liés à la dépréciation de TLS 1.0/1.1. Pour plus d'informations, voir :

- [Préparation de TLS 1.2 dans Office 365 et Office 365 Cloud de la communauté du secteur public](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Les clients Windows 7 SP1/Windows 8 doivent activer TLS1.2. Pour plus d’informations, consultez des[Erreurs d’authentification se produisent lorsque le client n’a pas de prise en charge TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Installez KB3140245 et créez la valeur de registre. Pour plus d’informations, consultez  [Mise à jour pour activer TLS 1.1 et TLS 1.2 en tant que protocoles sécurisés par défaut dans WinHTTP dans Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Les clients Windows 7 SP1/Windows 8 doivent s’assurer que les suites de chiffrement TLS les plus récentes sont installées. Pour plus d’informations, consultez [Avis de sécurité Microsoft 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


