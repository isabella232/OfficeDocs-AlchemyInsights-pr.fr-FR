---
title: Expiration du certificat de Fédération ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398338"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiration du certificat de Fédération ADFS

Pour résoudre ce problème, procédez comme suit:
  
1. Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l'ordinateur (si le module n'est pas déjà installé). Pour ce faire, accédez à [gestion d'Azure ad à l'aide de Windows PowerShell](https://aka.ms/aadposh).
    
2. Suivez les étapes de la section «scénario 1: la section «expiration du certificat de signature de jetons AD FS» du message [«il y a eu un problème d'accès au site» à partir d'AD FS lorsqu'un utilisateur fédéré se connecte à Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Suivez les étapes de [mise à jour ou de réparation des paramètres d'un domaine fédéré dans Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Pour en savoir plus sur le renouvellement des certificats de Fédération, consultez la rubrique [renouveler des certificats de Fédération pour Office 365 et Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

