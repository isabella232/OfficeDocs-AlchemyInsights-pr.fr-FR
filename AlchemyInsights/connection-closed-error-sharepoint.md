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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233424"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="2b2dc-102">Erreur « La connexion sous-jacente a été fermée » dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="2b2dc-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="2b2dc-p101">Si vous recevez l’erreur « La connexion sous-jacente a été fermée » dans SharePoint, cela peut être lié au retrait de TLS 1.0/1.1. Pour plus d’informations, consultez ces articles :</span><span class="sxs-lookup"><span data-stu-id="2b2dc-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="2b2dc-105">Préparation de TLS 1.2 dans Office 365 et Office 365 Cloud de la communauté du secteur public</span><span class="sxs-lookup"><span data-stu-id="2b2dc-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="2b2dc-106">Des erreurs d’authentification se produisent si le client n’a pas de prise en charge TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="2b2dc-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="2b2dc-107">Si des utilisateurs utilisent Windows 7, assurez-vous qu’ils vérifient les [Suites de chiffrement TLS dans Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="2b2dc-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>