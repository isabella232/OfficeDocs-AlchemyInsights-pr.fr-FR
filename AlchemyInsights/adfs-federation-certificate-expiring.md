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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737187"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiration du certificat de Fédération ADFS

Pour résoudre ce problème, procédez comme suit :
  
1. Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l’ordinateur (si le module n’est pas déjà installé). Pour ce faire, accédez à [gestion d’Azure ad à l’aide de Windows PowerShell](https://aka.ms/aadposh).

2. Suivez les étapes de la section « scénario 1 : la section «expiration du certificat de signature de jetons AD FS » du message [« il y a eu un problème d’accès au site » à partir d’AD FS lorsqu’un utilisateur fédéré se connecte à Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Suivez les étapes décrites dans la [section mettre à jour ou réparer les paramètres d’un domaine fédéré dans Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Pour en savoir plus sur le renouvellement des certificats de Fédération, consultez la rubrique [renouveler des certificats de Fédération pour Office 365 et Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
