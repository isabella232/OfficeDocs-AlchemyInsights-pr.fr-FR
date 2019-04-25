---
title: L'un de vos certificats de service de Fédération sur site arrive à expiration
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419690"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>L'un de vos certificats de service de Fédération sur site arrive à expiration

Pour résoudre ce problème, procédez comme suit:
  
- Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l'ordinateur (si le module n'est pas déjà installé). Pour ce faire, accédez à [Azure Active Directory PowerShell pour Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Suivez les étapes de la section «scénario 1: la section «expiration du certificat de signature de jetons AD FS» du message [«il y a eu un problème d'accès au site» à partir d'AD FS lorsqu'un utilisateur fédéré se connecte à Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Suivez les étapes de la[procédure de mise à jour ou de réparation des paramètres d'un domaine fédéré dans Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Pour plus d'informations sur le renouvellement des certificats de Fédération, consultez la rubrique [renouvellement de certificat pour O365 et Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

