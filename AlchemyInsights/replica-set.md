---
title: Jeu de réplicas
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716270"
---
# <a name="replica-set"></a><span data-ttu-id="9afc1-102">Jeu de réplicas</span><span class="sxs-lookup"><span data-stu-id="9afc1-102">Replica set</span></span>

<span data-ttu-id="9afc1-103">AADDS est également appelé domaine géré.</span><span class="sxs-lookup"><span data-stu-id="9afc1-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="9afc1-104">Il s’agit en fait de deux contrôleurs de domaine qui sont exécutés et gérés par le back-end.</span><span class="sxs-lookup"><span data-stu-id="9afc1-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="9afc1-105">Les deux DCS incluent un DC principal et un DC de réplication.</span><span class="sxs-lookup"><span data-stu-id="9afc1-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="9afc1-106">Les sauvegardes dans AADDS (domaine géré) sont un processus automatisé géré par la plateforme Azure.</span><span class="sxs-lookup"><span data-stu-id="9afc1-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="9afc1-107">En cas de problème avec votre domaine géré, le support Azure peut vous aider à restaurer à partir d’une sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="9afc1-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="9afc1-108">Vous créez chaque jeu de réplicas dans un réseau virtuel.</span><span class="sxs-lookup"><span data-stu-id="9afc1-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="9afc1-109">Chaque réseau virtuel doit être homologue à tous les autres réseaux virtuels qui hébergent le jeu de réplicas d’un domaine géré.</span><span class="sxs-lookup"><span data-stu-id="9afc1-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="9afc1-110">Cette configuration crée une topologie de réseau de maillage qui prend en charge la réplication d’annuaires.</span><span class="sxs-lookup"><span data-stu-id="9afc1-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="9afc1-111">Un réseau virtuel peut prendre en charge plusieurs jeux de réplicas, à condition que chaque jeu de réplicas se trouve dans un sous-réseau virtuel différent.</span><span class="sxs-lookup"><span data-stu-id="9afc1-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="9afc1-112">Pour plus d’informations sur le jeu de réplicas, voir Ensembles de [réplicas de concepts.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="9afc1-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
