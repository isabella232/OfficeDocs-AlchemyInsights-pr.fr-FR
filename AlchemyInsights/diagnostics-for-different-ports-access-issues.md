---
title: Diagnostics pour différents problèmes d’accès aux ports
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897616"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="1a727-102">Diagnostics pour différents problèmes d’accès aux ports</span><span class="sxs-lookup"><span data-stu-id="1a727-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="1a727-103">Pour résoudre les différents problèmes d’accès aux ports, effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="1a727-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="1a727-104">Arrêtez/deallocatez la machine virtuelle (VM) à partir du portail, redémarrez la VM et testez à nouveau.</span><span class="sxs-lookup"><span data-stu-id="1a727-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="1a727-105">Contrôlez les paramètres réseau de votre VM pour déterminer si des groupes de sécurité réseau (NSG) bloquent le trafic.</span><span class="sxs-lookup"><span data-stu-id="1a727-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="1a727-106">Vous pouvez également utiliser [Outil de vérification du flux IP de Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) pour vérifier si les NSG bloquent le trafic, les itinéraires définis par l’utilisateur qui achemine votre trafic vers l’itinéraire local (« Chemin par défaut » 0.0.0.0/0) ou vers un équipement réseau.</span><span class="sxs-lookup"><span data-stu-id="1a727-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="1a727-107">Si vous rencontrez toujours des problèmes après avoir essayé les étapes ci-dessus, veuillez fournir le nom de la VM et le port TCP sur lequel vous essayez d'envoyer du courrier pour un diagnostic plus approfondi.</span><span class="sxs-lookup"><span data-stu-id="1a727-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="1a727-108">**Documents recommandés**</span><span class="sxs-lookup"><span data-stu-id="1a727-108">**Recommended Documents**</span></span>

[<span data-ttu-id="1a727-109">Limitations et recommandations pour l’envoi de messages sortants sur le port 25</span><span class="sxs-lookup"><span data-stu-id="1a727-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)