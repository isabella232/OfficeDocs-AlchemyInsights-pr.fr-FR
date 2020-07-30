---
title: Problèmes liés au réseau privé virtuel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505188"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="5ec29-102">Problèmes liés au réseau privé virtuel</span><span class="sxs-lookup"><span data-stu-id="5ec29-102">VPN related issues</span></span>

<span data-ttu-id="5ec29-103">L’implémentation réussie de la connectivité VPN pour les clients de la gestion des périphériques mobiles dépend d’un profil déployé qui reflète correctement les exigences de l’infrastructure VPN.</span><span class="sxs-lookup"><span data-stu-id="5ec29-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="5ec29-104">Pour connaître les paramètres appropriés pour les plateformes client que vous examinez, consultez :</span><span class="sxs-lookup"><span data-stu-id="5ec29-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="5ec29-105">Paramètres des appareils Windows 10 et Windows holographiques pour ajouter des connexions VPN à l’aide de Intune</span><span class="sxs-lookup"><span data-stu-id="5ec29-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="5ec29-106">Ajouter des paramètres VPN sur les appareils iOS et iPad dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5ec29-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="5ec29-107">Paramètres de l’appareil Android pour configurer le VPN dans Intune</span><span class="sxs-lookup"><span data-stu-id="5ec29-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="5ec29-108">Ajouter des paramètres VPN sur les appareils macOS dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5ec29-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="5ec29-109">Si votre profil VPN utilise l’authentification basée sur les certificats, assurez-vous que les profils de certificats racine et d’authentification de client liés au profil VPN sont correctement déployés.</span><span class="sxs-lookup"><span data-stu-id="5ec29-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="5ec29-110">**Problèmes courants**</span><span class="sxs-lookup"><span data-stu-id="5ec29-110">**Common Issues**</span></span>

<span data-ttu-id="5ec29-111">**J’ai déployé un profil réseau privé virtuel sur un appareil. Intune indique qu’il a réussi, mais que l’appareil ne se connecte pas au réseau privé virtuel.**</span><span class="sxs-lookup"><span data-stu-id="5ec29-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="5ec29-112">L’état réussite indique que Intune a correctement déployé le profil configuré.</span><span class="sxs-lookup"><span data-stu-id="5ec29-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="5ec29-113">Toutefois, il est possible que ces configurations ne correspondent pas à votre réseau ou d’autres exigences d'authentification.</span><span class="sxs-lookup"><span data-stu-id="5ec29-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="5ec29-114">Consultez les journaux dans le service d’infrastructure et d’authentification (sur le serveur VPN et le serveur NPS/RADIUS) pour plus d’informations sur la tentative de connexion.</span><span class="sxs-lookup"><span data-stu-id="5ec29-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="5ec29-115">Il se peut que vous deviez collaborer avec l’équipe de votre infrastructure réseau ou le fournisseur VPN tiers pour recueillir et consulter les journaux.</span><span class="sxs-lookup"><span data-stu-id="5ec29-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="5ec29-116">**Lorsque je configure un réseau privé virtuel (VPN) personnalisé pour iOS, la fonctionnalité VPN par application n’est pas mise à disposition.**</span><span class="sxs-lookup"><span data-stu-id="5ec29-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="5ec29-117">Le VPN par application pour les appareils iOS dans Intune est actuellement disponible pour une liste spécifique de fournisseurs et de partenaires, qui doivent également satisfaire les conditions préalables requises pour configurer un VPN par application.</span><span class="sxs-lookup"><span data-stu-id="5ec29-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="5ec29-118">Pour plus d’informations, consultez [Configurer le réseau privé virtuel (VPN) par application pour les appareils iOS/iPad dans Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="5ec29-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="5ec29-119">Pour plus d’informations sur tous les types de connexions VPN dans Intune, consultez [Créer des profils VPN pour se connecter aux serveurs VPN dans Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="5ec29-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="5ec29-120">\*\* Le VPN à la demande d'iOS ne se déclenche pas lors de l'accès à un domaine configuré\*\*</span><span class="sxs-lookup"><span data-stu-id="5ec29-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="5ec29-121">Pour tester les paramètres VPN automatiques, configurez les valeurs suivantes :</span><span class="sxs-lookup"><span data-stu-id="5ec29-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="5ec29-122">Je veux effectuer les opérations suivantes : **évaluer chaque tentative de connexion**</span><span class="sxs-lookup"><span data-stu-id="5ec29-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="5ec29-123">Indiquez si vous voulez vous connecter : **se connecter si nécessaire**</span><span class="sxs-lookup"><span data-stu-id="5ec29-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="5ec29-124">Lorsque les utilisateurs accèdent à ces domaines : **cible** *nom de domaine*</span><span class="sxs-lookup"><span data-stu-id="5ec29-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="5ec29-125">Si la configuration ci-dessus échoue, ajoutez l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="5ec29-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="5ec29-126">Lorsque cette URL est inaccessible, forcez la connexion du VPN : **BADURL**</span><span class="sxs-lookup"><span data-stu-id="5ec29-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>