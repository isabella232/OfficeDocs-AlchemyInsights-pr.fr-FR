---
title: L'un de vos certificats de service de fédération local arrive à expiration
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
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810050"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="81c9c-102">L'un de vos certificats de service de fédération local arrive à expiration</span><span class="sxs-lookup"><span data-stu-id="81c9c-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="81c9c-103">Pour résoudre ce problème, suivez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="81c9c-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="81c9c-104">Installez le module Microsoft Azure Active Directory pour Windows PowerShell sur l'ordinateur (si le module n'est pas déjà installé).</span><span class="sxs-lookup"><span data-stu-id="81c9c-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="81c9c-105">Pour ce faire, allez [à Azure Active Directory PowerShell pour Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="81c9c-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="81c9c-106">Suivez les étapes de la section « Scénario 1 : le certificat de signature de jetons AD FS a expiré » de l'erreur « Un problème s'est produit lors de l'accès au site » d'AD FS lorsqu'un utilisateur fédéré se signe à [Microsoft 365, Azure ou Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="81c9c-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="81c9c-107">Suivez les étapes de la procédure de mise à jour ou de réparation des paramètres d'un domaine fédéré dans [Microsoft 365, Azure ou Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="81c9c-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="81c9c-108">Pour plus d'informations sur le renouvellement des certificats de fédération, voir Renouvellement du certificat [pour O365 et Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="81c9c-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

