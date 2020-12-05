---
title: Prise en charge de Microsoft Edge pour Microsoft Defender application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576546"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="7c95f-102">Prise en charge de Microsoft Edge pour Microsoft Defender application Guard</span><span class="sxs-lookup"><span data-stu-id="7c95f-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="7c95f-103">Conçu pour Windows 10 et Microsoft Edge, application Guard utilise une approche d’isolation matérielle qui permet à un utilisateur de naviguer dans un site non approuvé depuis un conteneur isolé Hyper-V, séparé du système d’exploitation hôte.</span><span class="sxs-lookup"><span data-stu-id="7c95f-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="7c95f-104">Un administrateur d’entreprise définit une liste de sites Web approuvés, de ressources Cloud et de réseaux internes.</span><span class="sxs-lookup"><span data-stu-id="7c95f-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="7c95f-105">Lorsqu’un utilisateur visite un site qui ne figure pas dans la liste, Microsoft Edge ouvre le site dans le conteneur.</span><span class="sxs-lookup"><span data-stu-id="7c95f-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="7c95f-106">Cela signifie que si le site s’avère malveillant, le PC hôte restera protégé et l’agresseur n’obtiendra pas les données de l’entreprise.</span><span class="sxs-lookup"><span data-stu-id="7c95f-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="7c95f-107">L’installation des extensions dans le conteneur est prise en charge à partir de la version 81 de Microsoft Edge et elle peut être contrôlée via une stratégie.</span><span class="sxs-lookup"><span data-stu-id="7c95f-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="7c95f-108">L’adresse updateURL qui est utilisée dans la stratégie ExtensionInstallForcelist doit être ajoutée en tant que ressource neutre dans les stratégies d’isolation réseau utilisées par application Guard.</span><span class="sxs-lookup"><span data-stu-id="7c95f-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="7c95f-109">Pour plus d’informations, consultez la rubrique [prise en charge de Microsoft Edge pour Microsoft Defender application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="7c95f-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
