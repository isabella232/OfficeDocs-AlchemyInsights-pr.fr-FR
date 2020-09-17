---
title: Utiliser TeamViewer pour gérer à distance les appareils Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798446"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="0135f-102">Utiliser TeamViewer pour gérer à distance les appareils Intune</span><span class="sxs-lookup"><span data-stu-id="0135f-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="0135f-103">Les appareils gérés par Intune peuvent être administrés à distance à l’aide de [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="0135f-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="0135f-104">Pour gérer Intune à l’aide de TeamViewer, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="0135f-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="0135f-105">Commencez par obtenir les informations d’identification de TeamViewer pour configurer le connecteur TeamViewer sur Intune.</span><span class="sxs-lookup"><span data-stu-id="0135f-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="0135f-106">Cela permet à l’administrateur d’entrer des informations d’identification dans l’interface utilisateur du connecteur TeamViewer sous Appareils, une opération ponctuelle pour établir le lien entre Intune et le service TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="0135f-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="0135f-107">**Partie 1 : démarrer une session avec un appareil distant**</span><span class="sxs-lookup"><span data-stu-id="0135f-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="0135f-108">Sous **Tous les appareils**, sélectionnez l’appareil avec lequel vous voulez démarrer une session à distance.</span><span class="sxs-lookup"><span data-stu-id="0135f-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="0135f-109">À partir de **... Plus**, sélectionnez **Nouvelle session d’assistance à distance**.</span><span class="sxs-lookup"><span data-stu-id="0135f-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="0135f-110">Sélectionnez **Oui** pour confirmer que vous voulez établir une session à distance.</span><span class="sxs-lookup"><span data-stu-id="0135f-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="0135f-111">Une fois que la demande « Lancer une nouvelle session à distance » est reconnue par le service TeamViewer, une option vous permettant de **Démarrer l’assistance à distance** s’affiche sous les détails du volet Vue d’ensemble (ou, Essentiels) pour l’appareil.</span><span class="sxs-lookup"><span data-stu-id="0135f-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="0135f-112">Sélectionnez **Afficher plus** pour développer le volet et afficher l’état de l’assistance à distance.</span><span class="sxs-lookup"><span data-stu-id="0135f-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="0135f-113">Sélectionnez **Démarrer une session à distance** pour démarrer la session côté administrateur.</span><span class="sxs-lookup"><span data-stu-id="0135f-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="0135f-114">Choisissez de télécharger le fichier binaire TeamViewer (Windows), puis sélectionnez **Exécuter**.</span><span class="sxs-lookup"><span data-stu-id="0135f-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="0135f-115">**Remarque** vous pouvez ignorer toute page de navigateur web ouverte sur le site web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="0135f-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="0135f-116">Accusez réception de la demande d’application TeamViewer pour apporter des modifications sur l’appareil (Windows uniquement).</span><span class="sxs-lookup"><span data-stu-id="0135f-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="0135f-117">L’application TeamViewer démarre et inclut le code de session authentifiant la connexion avec l’appareil distant.</span><span class="sxs-lookup"><span data-stu-id="0135f-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="0135f-118">**Partie 2 : sur l’appareil ciblé pour une session à distance**</span><span class="sxs-lookup"><span data-stu-id="0135f-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="0135f-119">Ouvrez le Portail d’entreprise Intune.</span><span class="sxs-lookup"><span data-stu-id="0135f-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="0135f-120">Recherchez un indicateur de notification : « Votre administrateur informatique demande le contrôle de cet appareil pour une session d’assistance à distance », puis sélectionnez la notification.</span><span class="sxs-lookup"><span data-stu-id="0135f-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="0135f-121">Choisissez de télécharger l’application TeamViewer, ou d’accuser réception du téléchargement de l’application TeamViewer à partir de l’App Store, puis sélectionnez **Exécuter**.</span><span class="sxs-lookup"><span data-stu-id="0135f-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="0135f-122">**Remarque** vous pouvez ignorer toute page de navigateur web ouverte sur le site web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="0135f-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="0135f-123">Accusez réception de la demande d’application TeamViewer pour apporter des modifications sur l’appareil (Windows uniquement).</span><span class="sxs-lookup"><span data-stu-id="0135f-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="0135f-124">L’application TeamViewer démarre et inclut le code de session authentifiant la connexion avec l’appareil distant.</span><span class="sxs-lookup"><span data-stu-id="0135f-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="0135f-125">Une fenêtre contextuelle vous demande si vous voulez autoriser le démarrage de la session.</span><span class="sxs-lookup"><span data-stu-id="0135f-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="0135f-126">**Remarque** les codes de session générés par le service TeamViewer sont à usage unique.</span><span class="sxs-lookup"><span data-stu-id="0135f-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="0135f-127">Si vous perdez la connexion, vous devez :</span><span class="sxs-lookup"><span data-stu-id="0135f-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="0135f-128">Fermer l’instance de l’application TeamViewer sur l’appareil distant et sur la station de travail d’administration.</span><span class="sxs-lookup"><span data-stu-id="0135f-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="0135f-129">Fermer le Portail de l’entreprise sur l’appareil distant.</span><span class="sxs-lookup"><span data-stu-id="0135f-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="0135f-130">Lancer une nouvelle session d’assistance à distance à partir du Portail d’administration.</span><span class="sxs-lookup"><span data-stu-id="0135f-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="0135f-131">Rouvrir le portail de l’entreprise sur l’appareil distant pour recevoir la nouvelle notification.</span><span class="sxs-lookup"><span data-stu-id="0135f-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="0135f-132">Télécharger et ouvrir l’application TeamViewer sur l’appareil distant et la station de travail d’administration, comme précédemment.</span><span class="sxs-lookup"><span data-stu-id="0135f-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>