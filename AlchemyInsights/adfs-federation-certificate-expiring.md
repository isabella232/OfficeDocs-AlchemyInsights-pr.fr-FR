---
title: Expiration du certificat de fédération ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952967"
---
# <a name="adfs-federation-certificate-expiring"></a>Expiration du certificat de fédération ADFS

Pour résoudre ce problème, suivez les étapes suivantes :
  
1. Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l’ordinateur (si le module n’est pas déjà installé). Pour ce faire, allez sur Gérer Azure AD à [l’aide Windows PowerShell](https://aka.ms/aadposh).

2. Suivez les étapes de la section « Scénario 1 : le certificat de signature de jetons AD FS a expiré » de l’erreur « Un problème s’est produit lors de l’accès au site » d’AD FS lorsqu’un utilisateur fédéré se signe à Microsoft 365, Azure ou [Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Suivez les étapes de mise à jour ou de réparation des paramètres d’un domaine fédéré [dans Microsoft, Azure ou Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Pour en savoir plus sur le renouvellement des certificats de fédération, voir Renouveler des [certificats](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)de fédération Microsoft 365 et Azure Active Directory .
