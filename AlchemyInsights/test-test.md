---
title: Termes manquants dans le magasin de termes SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750449"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="c89ee-102">Activation du chiffrement BitLocker avec Intune</span><span class="sxs-lookup"><span data-stu-id="c89ee-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="c89ee-103">La stratégie de protection du point de terminaison Intune peut être utilisée pour configurer les paramètres de chiffrement Boitlocker pour les appareils Windows, comme décrit dans les paramètres suivants : Windows10 (et versions ultérieures) pour protéger les appareils à l’aide d’Intune</span><span class="sxs-lookup"><span data-stu-id="c89ee-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="c89ee-104">Vous devez savoir que de nombreux appareils plus récents exécutant Windows 10 prennent en charge le chiffrement BitLocker automatique, qui est déclenché sans l’application de la stratégie MDM.</span><span class="sxs-lookup"><span data-stu-id="c89ee-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="c89ee-105">Cela peut avoir un impact sur l’application de la stratégie si des paramètres autres que ceux par défaut sont configurés.</span><span class="sxs-lookup"><span data-stu-id="c89ee-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="c89ee-106">Pour plus d’informations, voir le Forum aux questions.</span><span class="sxs-lookup"><span data-stu-id="c89ee-106">See FAQ for more detail.</span></span>


<span data-ttu-id="c89ee-107">FAQ   Q : Quelles éditions de Windows prennent en charge le chiffrement des appareils à l’aide de la stratégie de protection du point de terminaison ?</span><span class="sxs-lookup"><span data-stu-id="c89ee-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="c89ee-108"> A : les paramètres de la stratégie de protection du point de terminaison Intune sont implémentés à l’aide du CSP BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c89ee-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="c89ee-109">Toutes les éditions et les versions de Windows ne prennent pas en charge le fournisseur de services cryptographiques BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="c89ee-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="c89ee-110">Pour le moment, les éditions Windows : entreprise ; Éducation, mobile, mobile Enterprise et professionnel (à partir de la build 1809 et versions ultérieures) sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="c89ee-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="c89ee-111">Q : si un appareil est déjà chiffré avec BitLocker à l’aide des paramètres de système d’exploitation par défaut pour la méthode de chiffrement et la force de chiffrement (XTS-AES-128), l’application d’une stratégie avec différents paramètres déclenchera automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?</span><span class="sxs-lookup"><span data-stu-id="c89ee-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="c89ee-112">R : Non.</span><span class="sxs-lookup"><span data-stu-id="c89ee-112">A: No.</span></span> <span data-ttu-id="c89ee-113">Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.</span><span class="sxs-lookup"><span data-stu-id="c89ee-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="c89ee-114">Remarque pour les appareils en cours d’enregistrement avec AutoPilot, le chiffrement automatique qui se produit pendant OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation.</span><span class="sxs-lookup"><span data-stu-id="c89ee-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="c89ee-115">Q si un périphérique est chiffré suite à l’application de la stratégie Intune sera-t-il déchiffré lors de la suppression de cette stratégie ?</span><span class="sxs-lookup"><span data-stu-id="c89ee-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="c89ee-116">A : la suppression de la stratégie liée au chiffrement n’entraîne pas le déchiffrement des lecteurs qui ont été configurés.</span><span class="sxs-lookup"><span data-stu-id="c89ee-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="c89ee-117">Q : pourquoi la stratégie de conformité Intune indique-t-elle que mon appareil ne dispose pas de « BitLocker Enabled », mais c’est ?</span><span class="sxs-lookup"><span data-stu-id="c89ee-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="c89ee-118">A : le paramètre « BitLocker Enabled » dans la stratégie de conformité Intune utilise le client Windows Device Health attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="c89ee-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="c89ee-119">Ce client mesure uniquement l’état de l’appareil au moment du démarrage.</span><span class="sxs-lookup"><span data-stu-id="c89ee-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="c89ee-120">Par conséquent, si un périphérique n’a pas été redémarré depuis le chiffrement BitLocker, le service client DHA ne signalera pas BitLocker comme étant actif.</span><span class="sxs-lookup"><span data-stu-id="c89ee-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>