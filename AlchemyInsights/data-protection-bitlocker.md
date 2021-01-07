---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768815"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="69f56-102">Activation du chiffrement BitLocker avec Intune</span><span class="sxs-lookup"><span data-stu-id="69f56-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="69f56-103">La stratégie de protection du point de terminaison Intune peut être utilisée pour configurer les paramètres de chiffrement BitLocker pour les appareils Windows.</span><span class="sxs-lookup"><span data-stu-id="69f56-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="69f56-104">Pour plus d’informations, voir [Paramètres Windows 10 (et versions ultérieures) pour protéger les appareils à l’aide d’Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="69f56-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="69f56-105">Vous devez savoir que de nombreux appareils plus récents exécutant Windows 10 prennent en charge le chiffrement BitLocker automatique, qui est déclenché sans l’application de la stratégie MDM.</span><span class="sxs-lookup"><span data-stu-id="69f56-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="69f56-106">Cela peut avoir un impact sur l’application de la stratégie si des paramètres autres que ceux par défaut sont configurés.</span><span class="sxs-lookup"><span data-stu-id="69f56-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="69f56-107">Pour plus d’informations, consultez le Forum aux questions suivant.</span><span class="sxs-lookup"><span data-stu-id="69f56-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="69f56-108">Pour plus d’informations sur la résolution des problèmes liés à BitLocker, voir [Troubleshoot BitLocker Policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="69f56-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="69f56-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="69f56-109">**FAQ**</span></span>

<span data-ttu-id="69f56-110">Q : Quelles éditions de Windows prennent en charge le chiffrement des appareils à l’aide de la stratégie de protection du point de terminaison ?</span><span class="sxs-lookup"><span data-stu-id="69f56-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="69f56-111">A : les paramètres de la stratégie de protection du point de terminaison Intune sont implémentés à l’aide du [CSP BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="69f56-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="69f56-112">Toutes les éditions ou les versions de Windows ne prennent pas en charge le fournisseur de services cryptographiques BitLocker.</span><span class="sxs-lookup"><span data-stu-id="69f56-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="69f56-113">Q : Comment BitLocker peut-il être activé sur les appareils sans intervention de l’utilisateur final ?</span><span class="sxs-lookup"><span data-stu-id="69f56-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="69f56-114">A : tant que les conditions préalables requises sont remplies, il est possible d’activer le « chiffrement silencieux » BitLocker via Intune.</span><span class="sxs-lookup"><span data-stu-id="69f56-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="69f56-115">Voir les détails des exigences en matière de périphériques et des exemples de paramètres de stratégie pour activer le chiffrement silencieux dans le document suivant : [activer le chiffrement BitLocker en mode silencieux](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="69f56-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="69f56-116">Q : si un appareil est déjà chiffré avec BitLocker à l’aide des paramètres de système d’exploitation par défaut pour la méthode de chiffrement et le niveau de chiffrement (XTS-AES-128), l’application d’une stratégie avec différents paramètres déclenchera automatiquement le rechiffrement du lecteur avec les nouveaux paramètres ?</span><span class="sxs-lookup"><span data-stu-id="69f56-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="69f56-117">R : Non.</span><span class="sxs-lookup"><span data-stu-id="69f56-117">A: No.</span></span> <span data-ttu-id="69f56-118">Pour appliquer les nouveaux paramètres de chiffrement, le lecteur doit d’abord être déchiffré.</span><span class="sxs-lookup"><span data-stu-id="69f56-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="69f56-119">**Remarque :** Pour les appareils en cours d’enregistrement avec AutoPilot, le chiffrement automatique qui se produit pendant OOBE n’est déclenché qu’une fois la stratégie Intune évaluée, ce qui permet d’utiliser les paramètres basés sur la stratégie à la place des valeurs par défaut du système d’exploitation.</span><span class="sxs-lookup"><span data-stu-id="69f56-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="69f56-120">Q : si un périphérique est chiffré à la suite de l’application de la stratégie Intune, sera-t-il déchiffré lors de la suppression de cette stratégie ?</span><span class="sxs-lookup"><span data-stu-id="69f56-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="69f56-121">A : la suppression de la stratégie liée au chiffrement n’entraîne pas le déchiffrement des lecteurs qui ont été configurés.</span><span class="sxs-lookup"><span data-stu-id="69f56-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="69f56-122">Q : pourquoi la stratégie de conformité Intune indique-t-elle que BitLocker n’est pas activé sur mon appareil, même s’il s’agit de ?</span><span class="sxs-lookup"><span data-stu-id="69f56-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="69f56-123">A : le paramètre « BitLocker Enabled » dans la stratégie de conformité Intune utilise le client Windows Device Health attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="69f56-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="69f56-124">Ce client mesure uniquement l’état de l’appareil au moment du démarrage.</span><span class="sxs-lookup"><span data-stu-id="69f56-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="69f56-125">Par conséquent, si un périphérique n’a pas été redémarré depuis le chiffrement BitLocker terminé, le service client DHA ne signalera pas BitLocker comme étant actif.</span><span class="sxs-lookup"><span data-stu-id="69f56-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 