---
title: Expiration du certificat de Fédération ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710405"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="846c9-102">Expiration du certificat de Fédération ADFS</span><span class="sxs-lookup"><span data-stu-id="846c9-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="846c9-103">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="846c9-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="846c9-104">Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l’ordinateur (si le module n’est pas déjà installé).</span><span class="sxs-lookup"><span data-stu-id="846c9-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="846c9-105">Pour ce faire, accédez à [gestion d’Azure ad à l’aide de Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="846c9-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="846c9-106">Suivez les étapes de la section « scénario 1 : la section «expiration du certificat de signature de jetons AD FS » du message [« il y a eu un problème d’accès au site » à partir d’AD FS lorsqu’un utilisateur fédéré se connecte à Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="846c9-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="846c9-107">Suivez les étapes décrites dans la [section mettre à jour ou réparer les paramètres d’un domaine fédéré dans Microsoft, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="846c9-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="846c9-108">Pour en savoir plus sur le renouvellement des certificats de Fédération, consultez la rubrique [renouveler des certificats de Fédération pour Microsoft 365 et Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="846c9-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
