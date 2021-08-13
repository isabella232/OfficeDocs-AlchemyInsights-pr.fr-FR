---
title: L’un de vos certificats de service de fédération local arrive à expiration
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985215"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>L’un de vos certificats de service de fédération local arrive à expiration

Pour résoudre ce problème, suivez les étapes suivantes :
  
- Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l’ordinateur (si le module n’est pas déjà installé). Pour ce faire, Azure Active Directory [PowerShell pour Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Suivez les étapes de la section « Scénario 1 : le certificat de signature de jetons AD FS a expiré » de l’erreur « Un problème s’est produit lors de l’accès au site » d’AD FS lorsqu’un utilisateur fédéré se signe à Microsoft 365, Azure ou [Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Suivez les étapes de la procédure de mise à jour ou de réparation des paramètres d’un domaine fédéré [dans Microsoft 365, Azure ou Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Pour plus d’informations sur le renouvellement des certificats de fédération, voir Renouvellement du certificat [pour O365 et Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

