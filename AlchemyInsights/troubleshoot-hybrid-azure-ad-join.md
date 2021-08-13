---
title: Résoudre les problèmes de jointure Azure AD Hybride
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939269"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Résoudre les problèmes de jointure Azure AD Hybride

L’option Fortement recommandé permet à un appareil d’accéder aux points de terminaison de l’enregistrement des appareils sous le compte du système à l’aide de la fonction [Tester le script de connectivité de l’enregistrement des appareils](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Si vous configurez l’enregistrement des appareils pour la première fois, n’oubliez pas de consulter [Présentation de la gestion des appareils dans Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) pour mettre les appareils sous la gestion de d’Azure AD.
1. Si vous procédez à l’enregistrement d’appareils dans Azure AD et à leur inscription dans Intune, assurez-vous d’avoir [configuré Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) et d’avoir la [Licence](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) d’abord.
1. Assurez-vous que vous êtes autorisé à effectuer des opérations dans Azure AD et dans AD local. Seul un administrateur général dans Azure AD peut gérer les paramètres d’enregistrement des appareils. Par ailleurs, si vous configurez les enregistrements automatiques dans votre Active Directory local, vous devez être administrateur d’Active Directory et des services ADFS (le cas échéant).

Pour plus d’informations sur la résolution des problèmes potentiels avec la jonction hybride, consultez [Résoudre les problèmes de jonction hybride](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Pour configurer la Jointure hybride Azure AD et la Gestion des appareils à l’aide du portail Azure Ad, consultez [Configurer la jointure hybride Azure AD des appareils (joints au domaine local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) et [Gérer des appareils à l’aide du portail Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Pour résoudre les problèmes courants liés à la jointure d’Azure Active Directory (AD) Hybride, voir la [FAQ sur la jointure Azure AD Hybride](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
