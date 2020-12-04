---
title: Résoudre les problèmes liés à PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571876"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="a5bf1-102">Résoudre les problèmes liés à PRT</span><span class="sxs-lookup"><span data-stu-id="a5bf1-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="a5bf1-103">Pour que tout appareil s’exécute authentifié, il doit être entièrement enregistré et en parfait état et capable d’acquérir un jeton d’actualisation principal (PRT).</span><span class="sxs-lookup"><span data-stu-id="a5bf1-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="a5bf1-104">Le processus d’inscription de jointure Azure AD hybride nécessite que les appareils soient sur un réseau d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="a5bf1-105">Il fonctionne également sur VPN, mais il existe quelques inconvénients à ce propos.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="a5bf1-106">Nous avons entendu des clients qui ont besoin d’aide pour résoudre les problèmes liés au processus d’inscription de participation à Azure AD hybride dans des conditions de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="a5bf1-107">Voici une ventilation de ce qui se passe « en coulisse » pendant le processus d’inscription.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="a5bf1-108">**Environnement d’authentification Cloud (à l’aide de l’authentification directe ou de synchronisation de hachage de mot de passe Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="a5bf1-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="a5bf1-109">Ce flux d’enregistrement est également appelé « jointure de synchronisation ».</span><span class="sxs-lookup"><span data-stu-id="a5bf1-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="a5bf1-110">Windows 10 identifie un enregistrement SCP lorsque l’utilisateur se connecte à l’appareil.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="a5bf1-111">Le périphérique tente d’abord de récupérer les informations client à partir du SCP côté client dans le registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="a5bf1-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="a5bf1-112">Pour plus d’informations, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="a5bf1-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="a5bf1-113">En cas d’échec, le périphérique communique avec Active Directory local (AD) pour obtenir les informations du client à partir du point de connexion de service (SCP).</span><span class="sxs-lookup"><span data-stu-id="a5bf1-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="a5bf1-114">Pour vérifier le SCP, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="a5bf1-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="a5bf1-115">Nous vous recommandons d’activer SCP dans AD et de n’utiliser que le SCP côté client pour la validation initiale.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="a5bf1-116">Windows 10 tente de communiquer avec Azure AD dans le contexte système pour s’authentifier auprès d’Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="a5bf1-117">Vous pouvez vérifier si l’appareil peut accéder aux ressources Microsoft sous le compte système à l’aide du script de test de connectivité de Device Registration.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="a5bf1-118">Windows 10 génère un certificat auto-signé et le stocke sous l’objet ordinateur dans AD locale.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="a5bf1-119">Cela nécessite une visibilité du contrôleur de domaine.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="a5bf1-120">Un objet périphérique qui a un certificat est synchronisé avec Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="a5bf1-121">Le cycle de synchronisation est défini toutes les 30 minutes par défaut, mais dépend de la configuration d’Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="a5bf1-122">Pour plus d’informations, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="a5bf1-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="a5bf1-123">À ce stade, vous devriez être en mesure d’afficher l’objet de l’objet dans l’État « en attente » sous Blade de périphérique d’Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="a5bf1-124">Lors de la connexion utilisateur suivante à Windows 10, l’inscription est effectuée.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="a5bf1-125">Si vous êtes sur un VPN et qu’un processus de fermeture de session ferme le domaine, vous pouvez déclencher l’inscription manuellement :</span><span class="sxs-lookup"><span data-stu-id="a5bf1-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="a5bf1-126">Émettez une invite dsregcmd/Join localement sur l’administrateur ou à distance via PSExec à votre PC.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="a5bf1-127">Par exemple, PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="a5bf1-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="a5bf1-128">Pour plus d’informations sur les problèmes de jointure hybride, consultez la rubrique [Troubleshoot Devices](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)problem.</span><span class="sxs-lookup"><span data-stu-id="a5bf1-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
