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
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753028"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="a82c2-102">L'un de vos certificats de service de Fédération sur site arrive à expiration</span><span class="sxs-lookup"><span data-stu-id="a82c2-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="a82c2-103">Pour résoudre ce problème, procédez comme suit:</span><span class="sxs-lookup"><span data-stu-id="a82c2-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="a82c2-104">Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l'ordinateur (si le module n'est pas déjà installé).</span><span class="sxs-lookup"><span data-stu-id="a82c2-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a82c2-105">Pour ce faire, accédez à [Azure Active Directory PowerShell pour Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="a82c2-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="a82c2-106">Suivez les étapes de la section «scénario 1: la section «expiration du certificat de signature de jetons AD FS» du message [«il y a eu un problème d'accès au site» à partir d'AD FS lorsqu'un utilisateur fédéré se connecte à Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a82c2-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="a82c2-107">Suivez les étapes de la[procédure de mise à jour ou de réparation des paramètres d'un domaine fédéré dans Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="a82c2-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="a82c2-108">Pour plus d'informations sur le renouvellement des certificats de Fédération, consultez la rubrique [renouvellement de certificat pour O365 et Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a82c2-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

