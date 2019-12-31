---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908708"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="50140-102">Activation du chiffrement BitLocker avec Intune</span><span class="sxs-lookup"><span data-stu-id="50140-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="50140-103">La stratégie de protection du point de terminaison Intune peut être utilisée pour configurer les paramètres de chiffrement BitLocker pour les appareils Windows.</span><span class="sxs-lookup"><span data-stu-id="50140-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="50140-104">Pour plus d’informations, voir [Paramètres Windows 10 (et versions ultérieures) pour protéger les appareils à l’aide d’Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="50140-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="50140-105">Vous devez savoir que de nombreux appareils plus récents exécutant Windows 10 prennent en charge le chiffrement BitLocker automatique, qui est déclenché sans l’application de la stratégie MDM.</span><span class="sxs-lookup"><span data-stu-id="50140-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="50140-106">Cela peut avoir un impact sur l’application de la stratégie si des paramètres autres que ceux par défaut sont configurés.</span><span class="sxs-lookup"><span data-stu-id="50140-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="50140-107">Pour plus d’informations, consultez le Forum aux questions suivant.</span><span class="sxs-lookup"><span data-stu-id="50140-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="50140-108">Pour plus d’informations sur la résolution des problèmes liés à BitLocker, voir [Troubleshoot BitLocker Policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="50140-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="50140-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="50140-109">**FAQ**</span></span>

 <span data-ttu-id="50140-110">Q : Quelles éditions de Windows prennent en charge le chiffrement des appareils à l’aide de la stratégie de protection du point de terminaison ?</span><span class="sxs-lookup"><span data-stu-id="50140-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="50140-111">A : les paramètres de la stratégie de protection du point de terminaison Intune sont implémentés à l’aide du [CSP BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="50140-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="50140-112">Toutes les éditions ou les versions de Windows ne prennent pas en charge le fournisseur de services cryptographiques BitLocker.</span><span class="sxs-lookup"><span data-stu-id="50140-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="50140-113">Pour l’instant, les éditions suivantes de Windows sont prises en charge : entreprise, éducation, mobile, mobile Enterprise et professionnel (Build 1809 et versions ultérieures).</span><span class="sxs-lookup"><span data-stu-id="50140-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="50140-114">Q : si un appareil est déjà chiffré avec BitLocker à l’aide des paramètres de système d’exploitation par défaut pour la méthode de chiffrement et le niveau de chiffrement (XTS-AES-128), l’application d’une stratégie avec différents paramètres déclenchera automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?</span><span class="sxs-lookup"><span data-stu-id="50140-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="50140-115">R : Non.</span><span class="sxs-lookup"><span data-stu-id="50140-115">A: No.</span></span> <span data-ttu-id="50140-116">Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.</span><span class="sxs-lookup"><span data-stu-id="50140-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="50140-117">**Remarque :** Pour les appareils en cours d’enregistrement avec AutoPilot, le chiffrement automatique qui se produit pendant OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation.</span><span class="sxs-lookup"><span data-stu-id="50140-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="50140-118">Q : si un périphérique est chiffré à la suite de l’application de la stratégie Intune, sera-t-il déchiffré lors de la suppression de cette stratégie ?</span><span class="sxs-lookup"><span data-stu-id="50140-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="50140-119">A : la suppression de la stratégie liée au chiffrement n’entraîne pas le déchiffrement des lecteurs qui ont été configurés.</span><span class="sxs-lookup"><span data-stu-id="50140-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="50140-120">Q : pourquoi la stratégie de conformité Intune indique-t-elle que BitLocker n’est pas activé sur mon appareil, même s’il s’agit de ?</span><span class="sxs-lookup"><span data-stu-id="50140-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="50140-121">A : le paramètre « BitLocker Enabled » dans la stratégie de conformité Intune utilise le client Windows Device Health attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="50140-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="50140-122">Ce client mesure uniquement l’état de l’appareil au moment du démarrage.</span><span class="sxs-lookup"><span data-stu-id="50140-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="50140-123">Par conséquent, si un périphérique n’a pas été redémarré depuis le chiffrement BitLocker terminé, le service client DHA ne signalera pas BitLocker comme étant actif.</span><span class="sxs-lookup"><span data-stu-id="50140-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 