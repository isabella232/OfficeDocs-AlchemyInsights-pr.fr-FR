---
title: Configuration virtuelle avec les services de domaine AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884580"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="f80c5-102">Configuration virtuelle avec les services de domaine AAD</span><span class="sxs-lookup"><span data-stu-id="f80c5-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="f80c5-103">La configuration virtuelle avec les services de domaine AAD comprend ces étapes :</span><span class="sxs-lookup"><span data-stu-id="f80c5-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="f80c5-104">La vérification de l’intégrité de votre domaine sur le portail Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="f80c5-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="f80c5-105">La recherche dans votre NSG des règles qui bloquent les ports nécessaires à la synchronisation dans les services de domaine Azure AD sur le portail https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="f80c5-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="f80c5-106">Vous assurer que votre réseau virtuel est déployé dans la même région Azure que le domaine géré par les services de domaine Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f80c5-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="f80c5-107">Vous assurer que vous n’avez pas de domaine existant avec le même nom de domaine disponible sur le réseau virtuel.</span><span class="sxs-lookup"><span data-stu-id="f80c5-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="f80c5-108">Pour plus d’informations sur les considérations en matière de conception sur Réseau Virtuel Azure afin de prendre en charge les services de domaine AAD, consultez[Considération du Réseau Virtuel](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="f80c5-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

