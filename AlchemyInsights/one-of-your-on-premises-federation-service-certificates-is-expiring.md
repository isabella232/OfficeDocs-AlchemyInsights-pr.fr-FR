---
title: Un de vos certificats de Service de fédération local arrive à expiration
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 9e2e1a1dd2993b2a02b4405db8a707b23ff4af16
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658905"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Un de vos certificats de Service de fédération local arrive à expiration

Pour résoudre ce problème, procédez comme suit :
  
- Installer le Microsoft Azure Active Directory Module pour Windows PowerShell sur l’ordinateur (si le module n’est pas déjà installé). Pour ce faire, accédez à [Windows Azure Active Directory PowerShell graphique](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Suivez les étapes décrites dans le « scénario 1 : expiration du certificat de signature de jetons AD FS » section de [l’erreur « Impossible de l’accès au site » AD FS lorsqu’un utilisateur fédéré se connecte à Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Suivez les étapes décrites dans t[comment mettre à jour ou réparer les paramètres d’un domaine fédéré dans Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Pour plus d’informations sur le renouvellement des certificats de fédération, voir [le renouvellement de certificat pour O365 et Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

