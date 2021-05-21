---
title: 401 Erreur non autorisée dans SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539930"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="c9890-102">401 Erreur non autorisée dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="c9890-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="c9890-p101">Si vous recevez l’erreur « (401) Non autorisé » dans SharePoint, elle peut être liée au retrait de TLS 1.0/1.1. Pour plus d’informations, consultez :</span><span class="sxs-lookup"><span data-stu-id="c9890-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

- [<span data-ttu-id="c9890-105">Préparation de TLS 1.2 dans Office 365 et Office 365 Cloud de la communauté du secteur public</span><span class="sxs-lookup"><span data-stu-id="c9890-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="c9890-106">Des erreurs d’authentification se produisent si le client n’a pas de prise en charge TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="c9890-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="c9890-107">Mise à jour pour activer TLS 1.1 et TLS 1.2 comme protocoles sécurisés par défaut dans WinHTTP sous Windows</span><span class="sxs-lookup"><span data-stu-id="c9890-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="c9890-108">Si des utilisateurs utilisent Windows 7, assurez-vous qu’ils vérifient les [Suites de chiffrement TLS dans Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="c9890-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>