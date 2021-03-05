---
title: Problème avec AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453292"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="fb485-102">Problème avec AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="fb485-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="fb485-103">Assurez-vous que vous êtes autorisé à effectuer l’opération.</span><span class="sxs-lookup"><span data-stu-id="fb485-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fb485-104">Les administrateurs globaux y ont accès par défaut.</span><span class="sxs-lookup"><span data-stu-id="fb485-104">Global Admins have access by default.</span></span> <span data-ttu-id="fb485-105">En outre, vous pouvez utiliser le contrôle [d’accès](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) basé sur un rôle pour déléguer l’autorisation d’inscription au collaborateur.</span><span class="sxs-lookup"><span data-stu-id="fb485-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fb485-106">Assurez-vous que les points de terminaison requis sont activés et non bloqués en raison du pare-feu.</span><span class="sxs-lookup"><span data-stu-id="fb485-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fb485-107">Pour plus d’informations, voir [les conditions requises.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="fb485-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fb485-108">L’inscription peut échouer en raison de la communication sortante soumise à l’inspection SSL par la couche réseau.</span><span class="sxs-lookup"><span data-stu-id="fb485-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fb485-109">Assurez-vous que vous avez vérifié les paramètres de notification pour Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="fb485-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="fb485-110">Veuillez consulter votre paramètre.</span><span class="sxs-lookup"><span data-stu-id="fb485-110">Please review your setting.</span></span> <span data-ttu-id="fb485-111">Ce [guide peut](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vous aider à comprendre comment configurer les paramètres de notification pour les notifications d’état d’état Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fb485-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="fb485-112">Pour en savoir plus sur le rapport de synchronisation aAD Connect Health et sur la façon de le télécharger, consultez le rapport de synchronisation au niveau [de l’objet.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="fb485-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fb485-113">Pour résoudre les problèmes d’alertes d’état AAD Connect, suivez le guide de dépannage pour les alertes d’actualité des données d’état [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) et pour les questions fréquemment posées, consultez les questions courantes sur l’installation [d’AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="fb485-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
