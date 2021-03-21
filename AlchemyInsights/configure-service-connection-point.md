---
title: Configurer le point de connexion de service (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897733"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="ebf2c-102">Configurer le point de connexion de service (SCP)</span><span class="sxs-lookup"><span data-stu-id="ebf2c-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="ebf2c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="ebf2c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="ebf2c-104">**Raison** : impossible de lire l’objet SCP et d’obtenir les informations du client Azure AD</span><span class="sxs-lookup"><span data-stu-id="ebf2c-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="ebf2c-105">**Résolution** : reportez-vous à la section [Configurer un point de connexion au service](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="ebf2c-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="ebf2c-106">**Plan d’action**</span><span class="sxs-lookup"><span data-stu-id="ebf2c-106">**Action plan**</span></span>

- <span data-ttu-id="ebf2c-107">Vérifiez si l’appareil a reçu l’objet de stratégie de groupe pour la validation contrôlée.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="ebf2c-108">Assurez-vous que l’objet de stratégie de groupe a créé les clés de Registre.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="ebf2c-109">Assurez-vous que vous avez deux clés créées avec votre ID d’annuaire et votre domaine onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="ebf2c-110">**Configurer le paramètre de Registre côté client pour le protocole SCP**</span><span class="sxs-lookup"><span data-stu-id="ebf2c-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="ebf2c-111">Utilisez l’exemple suivant pour créer un objet de stratégie de groupe afin de déployer un paramètre de Registre qui configure une entrée SCP dans le Registre de vos appareils.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="ebf2c-112">Ouvrez une console de gestion des stratégies de groupe et créez un nouveau groupe de stratégies de groupe dans votre domaine.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="ebf2c-113">Donnez un nom à votre objet de stratégie de groupe nouvellement créée (par exemple, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="ebf2c-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="ebf2c-114">Modifiez l'objet de stratégie de groupe et recherchez le chemin d'accès suivant : **Configuration de l’ordinateur > Préférences > Paramètres Windows > Registre**.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="ebf2c-115">Cliquez avec le bouton droit sur **Registre**, sélectionnez **Nouveau > Élément de Registre**.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="ebf2c-116">Dans l'onglet **Général**, configurez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ebf2c-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="ebf2c-117">**Action** : Mise à jour</span><span class="sxs-lookup"><span data-stu-id="ebf2c-117">**Action**: Update</span></span>
    
- <span data-ttu-id="ebf2c-118">**Hive** : HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="ebf2c-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="ebf2c-119">**Chemin d’accès** : SOFTWARE\Microsoft\Windows\CurrentVersion\C PATH\AAD</span><span class="sxs-lookup"><span data-stu-id="ebf2c-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="ebf2c-120">**Nom de la valeur** : TenantId</span><span class="sxs-lookup"><span data-stu-id="ebf2c-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="ebf2c-121">**Type de valeur** : REG_SZ</span><span class="sxs-lookup"><span data-stu-id="ebf2c-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="ebf2c-122">**Données de valeur** : GUID ou ID d’annuaire de votre instance Azure AD (cette valeur est dans **Portail Azure > Azure Active Directory > Propriétés > ID d’annuaire**)</span><span class="sxs-lookup"><span data-stu-id="ebf2c-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="ebf2c-123">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="ebf2c-124">Cliquez avec le bouton droit sur **Registre**, sélectionnez **Nouveau > Élément de Registre**.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="ebf2c-125">Dans l'onglet **Général**, configurez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ebf2c-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="ebf2c-126">**Action** : Mise à jour</span><span class="sxs-lookup"><span data-stu-id="ebf2c-126">**Action**: Update</span></span>
    
- <span data-ttu-id="ebf2c-127">**Hive** : HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="ebf2c-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="ebf2c-128">**Chemin d’accès** : SOFTWARE\Microsoft\Windows\CurrentVersion\C PATH\AAD</span><span class="sxs-lookup"><span data-stu-id="ebf2c-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="ebf2c-129">**Nom de la valeur** : TenantName</span><span class="sxs-lookup"><span data-stu-id="ebf2c-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="ebf2c-130">**Type de valeur** : REG_SZ</span><span class="sxs-lookup"><span data-stu-id="ebf2c-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="ebf2c-131">**Données de valeur** : votre nom de domaine vérifié si vous utilisez un environnement fédéré tel qu’AD FS.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="ebf2c-132">Votre nom de domaine vérifié ou votre nom de domaine onmicrosoft.com (par exemple, contoso.onmicrosoft.com si vous utilisez un environnement géré).</span><span class="sxs-lookup"><span data-stu-id="ebf2c-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="ebf2c-133">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-133">Click **OK**.</span></span>

7. <span data-ttu-id="ebf2c-134">Fermez l’éditeur du nouvel éditeur.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="ebf2c-135">Liez l’objet de stratégie de groupe nouvellement créé à l'OU souhaitée contenant les ordinateurs joints au domaine qui appartiennent à votre population de déploiement contrôlé.</span><span class="sxs-lookup"><span data-stu-id="ebf2c-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="ebf2c-136">Pour plus d’informations, consultez [Validation contrôlée de la jonction Azure AD Hybride - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) et [Résolution des problèmes des appareils joints Azure Active Directory hybrides | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="ebf2c-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









