---
title: Appareil en état d’attente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652191"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="ec8f6-102">Appareil en état d’attente</span><span class="sxs-lookup"><span data-stu-id="ec8f6-102">Device in pending state</span></span>

<span data-ttu-id="ec8f6-103">**Conditions préalables**</span><span class="sxs-lookup"><span data-stu-id="ec8f6-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="ec8f6-104">Si vous configurez les inscriptions d’appareils pour la première fois, vérifiez que vous avez lu la rubrique relative à la gestion des appareils [dans Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) pour vous aider à obtenir des périphériques sous le contrôle d’Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="ec8f6-105">Si vous enregistrez les appareils dans Azure AD directement et en les inscrivant dans Intune, vous devez vous assurer que vous avez [configuré Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) et que la gestion des [licences](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) est en place.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="ec8f6-106">Assurez-vous que vous êtes autorisé à effectuer des opérations dans Azure AD et AD sur site.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="ec8f6-107">Seul un administrateur général dans Azure AD peut gérer les paramètres des inscriptions d’appareils.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="ec8f6-108">En outre, si vous configurez des enregistrements automatiques dans votre annuaire Active Directory local, vous devez être un administrateur d’Active Directory et d’AD FS (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="ec8f6-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="ec8f6-109">Le processus d’inscription hybride Azure AD requiert des périphériques sur le réseau d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="ec8f6-110">Il fonctionne également sur VPN, mais il existe quelques inconvénients à ce propos.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="ec8f6-111">Nous avons entendu des clients qui ont besoin d’aide pour résoudre les problèmes liés au processus d’inscription hybride Azure AD dans des conditions de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="ec8f6-112">**Environnement d’authentification Cloud (à l’aide de l’authentification directe ou de synchronisation de hachage de mot de passe Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="ec8f6-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="ec8f6-113">Ce flux d’enregistrement est également appelé « jointure de synchronisation ».</span><span class="sxs-lookup"><span data-stu-id="ec8f6-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="ec8f6-114">Voici une répartition de ce qui se produit pendant le processus d’inscription :</span><span class="sxs-lookup"><span data-stu-id="ec8f6-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="ec8f6-115">Windows 10 identifie l’enregistrement du point de connexion de service (SCP) lorsque l’utilisateur se connecte à l’appareil.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="ec8f6-116">Le périphérique tente d’abord de récupérer les informations client à partir du SCP côté client dans le registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="ec8f6-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="ec8f6-117">Pour plus d’informations, consultez la rubrique [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="ec8f6-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="ec8f6-118">En cas d’échec, le périphérique communique avec Active Directory local pour obtenir les informations du client auprès du SCP.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="ec8f6-119">Pour vérifier le SCP, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="ec8f6-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="ec8f6-120">Nous vous recommandons d’activer SCP dans Active Directory et de n’utiliser que le SCP côté client pour la validation initiale.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="ec8f6-121">Windows 10 tente de communiquer avec Azure AD dans le contexte système pour s’authentifier auprès d’Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="ec8f6-122">Vous pouvez vérifier si l’appareil peut accéder aux ressources Microsoft sous le compte système à l’aide du [script de test de connectivité de Device Registration](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="ec8f6-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="ec8f6-123">Windows 10 génère un certificat auto-signé et le stocke sous l’objet ordinateur dans Active Directory en local.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="ec8f6-124">Cela nécessite une visibilité du contrôleur de domaine.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="ec8f6-125">L’objet appareil dont le certificat est synchronisé est synchronisé avec Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="ec8f6-126">Le cycle de synchronisation est défini toutes les 30 minutes par défaut, mais dépend de la configuration d’Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="ec8f6-127">Pour plus d’informations, reportez-vous à ce [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="ec8f6-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="ec8f6-128">À ce stade, vous devriez être en mesure d’afficher l’objet de l’objet dans l’état «**en attente**» sous Blade de périphérique d’Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="ec8f6-129">Lors de la connexion utilisateur suivante à Windows 10, l’inscription est effectuée.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ec8f6-130">Si vous êtes sur un VPN et que la déconnexion et la connexion se terminent, vous pouvez déclencher l’inscription manuellement.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="ec8f6-131">Pour cela :</span><span class="sxs-lookup"><span data-stu-id="ec8f6-131">To do that:</span></span>
    >
    > <span data-ttu-id="ec8f6-132">Émettez une `dsregcmd /join` invite locale sur l’administrateur ou à distance via PsExec à votre PC.</span><span class="sxs-lookup"><span data-stu-id="ec8f6-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="ec8f6-133">Par exemple : `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="ec8f6-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="ec8f6-134">Pour les problèmes courants liés à l’inscription d’appareils Azure Active Directory, consultez la rubrique [périphériques FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="ec8f6-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
