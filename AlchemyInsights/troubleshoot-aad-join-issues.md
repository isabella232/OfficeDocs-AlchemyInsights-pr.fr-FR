---
title: Résoudre les problèmes de jointation à Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939917"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Résoudre les problèmes de jointation à Azure AD

1. Si vous êtes en train de définir des inscriptions d’appareils pour la première fois, assurez-vous d’avoir examiné l’introduction à la gestion des appareils dans [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) qui vous guidera sur la façon d’obtenir les appareils sous le contrôle d’Azure AD. 
1. Si vous inscrivez des appareils directement dans Azure AD et que vous les inscrivez dans Intune, vous [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) devez vous assurer que vous avez configuré [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) et que la licence est en place en premier.
1. Assurez-vous que vous êtes autorisé à effectuer des opérations dans Azure AD. Seul un administrateur général dans Azure AD peut gérer les paramètres d’enregistrement des appareils.
1. Pour l’implémentation de la jointisation Azure AD, voir [Planifier Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Pour plus d’informations sur la résolution des problèmes courants avec la jointation Azure AD, consultez le FAQ sur azure [Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) et pour l’appareil professionnel Windows 10, voir Impossible de joindre un ordinateur Windows 10 Professionnel à [Azure AD -](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) Besoin de mettre à niveau vers - Microsoft Community
