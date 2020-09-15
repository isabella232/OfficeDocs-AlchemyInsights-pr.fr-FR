---
title: Expiration du certificat de fédération ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686712"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="f148f-102">Expiration du certificat de fédération ADFS</span><span class="sxs-lookup"><span data-stu-id="f148f-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="f148f-103">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="f148f-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="f148f-104">Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l’ordinateur (si le module n’est pas déjà installé).</span><span class="sxs-lookup"><span data-stu-id="f148f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f148f-105">Pour ce faire, accédez à [gestion d’Azure ad à l’aide de Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="f148f-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="f148f-106">Suivez les étapes de la section « scénario 1 : la section «expiration du certificat de signature de jetons AD FS » du message [« il y a eu un problème d’accès au site » à partir d’AD FS lorsqu’un utilisateur fédéré se connecte à Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="f148f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="f148f-107">Suivez les étapes décrites dans la [section mettre à jour ou réparer les paramètres d’un domaine fédéré dans Microsoft, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="f148f-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="f148f-108">Pour en savoir plus sur le renouvellement des certificats de Fédération, consultez la rubrique [renouveler des certificats de Fédération pour Microsoft 365 et Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="f148f-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
