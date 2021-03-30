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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403820"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Résoudre les problèmes de jointation à Azure AD

1. Si vous devez définir des inscriptions d’appareils pour la première fois, assurez-vous d’avoir examiné l’introduction à la gestion des appareils dans [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) qui vous guidera sur la façon d’obtenir des appareils sous le contrôle d’Azure AD. 
1. Si vous inscrivez des appareils directement dans Azure AD et que vous les inscrivez dans Intune, vous [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) devez vous assurer que vous avez configuré [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) et que la licence est en place en premier.
1. Assurez-vous que vous êtes autorisé à effectuer des opérations dans Azure AD. Seul un administrateur général dans Azure AD peut gérer les paramètres d’inscription des appareils.
1. Pour l’implémentation de la jointisation Azure AD, voir [Planifier Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Pour plus d’informations sur la résolution des problèmes courants avec la jointation Azure AD, consultez le FAQ sur azure [Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) et pour l’appareil Windows 10 Professionnel, voir Impossible de joindre l’ordinateur [Windows 10 Professionnel](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) à Azure AD - Besoin de mettre à niveau vers - Microsoft Community
