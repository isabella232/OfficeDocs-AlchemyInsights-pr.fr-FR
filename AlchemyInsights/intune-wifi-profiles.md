---
title: Profils Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509053"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="2d365-102">Profils Wi-Fi Intune</span><span class="sxs-lookup"><span data-stu-id="2d365-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="2d365-103">La mise en œuvre réussie de la connectivité Wi-Fi pour les clients de gestion des périphériques mobiles dépend d’un profil correctement déployé qui reflète les exigences de l’infrastructure Wi-Fi d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="2d365-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="2d365-104">Pour examiner les paramètres appropriés pour les plateformes client que vous examinez, voir :</span><span class="sxs-lookup"><span data-stu-id="2d365-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="2d365-105">Ajouter des paramètres Wi-Fi pour les appareils exécutant Android dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d365-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="2d365-106">Ajouter des paramètres Wi-Fi pour les appareils Android Enterprise dédiés et totalement gérés dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d365-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="2d365-107"> Ajouter les paramètres du Wi-Fi pour les appareils iOS et iPadOS dans Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d365-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="2d365-108">Ajouter des paramètres Wi-Fi pour les appareils Windows 10 et versions ultérieures dans Intune</span><span class="sxs-lookup"><span data-stu-id="2d365-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="2d365-109">Importer les paramètres Wi-Fi pour les appareils Windows dans Intune</span><span class="sxs-lookup"><span data-stu-id="2d365-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="2d365-110">**Problèmes courants**</span><span class="sxs-lookup"><span data-stu-id="2d365-110">**Common Issues**</span></span>

<span data-ttu-id="2d365-111">**Je déploie un profil Wi-Fi dépendant d’un certificat déployé spécifié dans le profil Wi-Fi. Toutefois, les profils de configuration affichent un état d’erreur.**</span><span class="sxs-lookup"><span data-stu-id="2d365-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="2d365-112">Vérifiez que votre appareil a reçu le certificat.</span><span class="sxs-lookup"><span data-stu-id="2d365-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="2d365-113">Dans Intune, accédez à **Tous les appareils** puis sélectionnez l’appareil > **Configuration de l’appareil**.</span><span class="sxs-lookup"><span data-stu-id="2d365-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="2d365-114">Vérifiez que tous les profils attendus sont répertoriés et que l’état de réussite est vérifié.</span><span class="sxs-lookup"><span data-stu-id="2d365-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="2d365-115">Pour un profil Android, si vous avez des certificats intermédiaires dans votre chaîne de certificats, assurez-vous qu’ils sont déployés sur les appareils Android.</span><span class="sxs-lookup"><span data-stu-id="2d365-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="2d365-116">Pour vérifier l’état du certificat, accédez à **Configuration des appareils** > **Profils** > **autorité intermédiaire** > **Propriétés** > **Certificat approuvé**.</span><span class="sxs-lookup"><span data-stu-id="2d365-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="2d365-117">Si vous continuez à rencontrer des erreurs, passez en revue les sections procédures et résolution des problèmes.</span><span class="sxs-lookup"><span data-stu-id="2d365-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="2d365-118">Pour plus d’informations, voir [Vue d’ensemble de la résolution des problèmes de profils de certificats SCEP avec Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2d365-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="2d365-119">**J’ai déployé un profil Wi-Fi sur un appareil. Intune indique qu’il a réussi, mais que l’appareil ne se connecte pas au Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="2d365-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="2d365-120">L’état réussite indique que Intune a correctement déployé le profil configuré.</span><span class="sxs-lookup"><span data-stu-id="2d365-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="2d365-121">Toutefois, il est possible que ces configurations ne correspondent pas à votre réseau ou d’autres exigences d'authentification.</span><span class="sxs-lookup"><span data-stu-id="2d365-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="2d365-122">Pour plus d’informations sur la tentative de connexion, passez en revue les journaux dans le service d’infrastructure et d’authentification (sur le contrôleur de point d’accès Wi-Fi et le serveur NPS/RADIUS).</span><span class="sxs-lookup"><span data-stu-id="2d365-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="2d365-123">Il se peut que vous deviez collaborer avec l’équipe de votre infrastructure réseau ou le fournisseur Wi-Fi tiers pour recueillir et consulter les journaux.</span><span class="sxs-lookup"><span data-stu-id="2d365-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>