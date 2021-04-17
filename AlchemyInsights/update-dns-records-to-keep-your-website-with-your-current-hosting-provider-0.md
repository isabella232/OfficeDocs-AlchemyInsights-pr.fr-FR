---
title: Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827514"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="3f572-102">Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel</span><span class="sxs-lookup"><span data-stu-id="3f572-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="3f572-103">Dans le Centre d'administration Microsoft 365, allez à la page Domaines   >  [](https://admin.microsoft.com/Adminportal#/Domains) d'installation et, dans la liste des domaines, sélectionnez le domaine que vous utilisez pour votre site web.</span><span class="sxs-lookup"><span data-stu-id="3f572-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="3f572-104">Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="3f572-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="3f572-105">Pour **Type de DNS** entrez : **A (Adresse)**</span><span class="sxs-lookup"><span data-stu-id="3f572-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="3f572-106">Pour **Nom d'hôte ou Alias**, tapez **@**.</span><span class="sxs-lookup"><span data-stu-id="3f572-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="3f572-107">Pour **Adresse IP**, tapez l'adresse IP statique correspondant à l'hébergement actuel de votre site web (par exemple, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="3f572-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="3f572-p101">Il doit s'agir d'une adresse IP  *statique*  pour le site web (et non d'une adresse IP  *dynamique*  ). Vérifiez l'emplacement d'hébergement de votre site web pour vous assurer que vous pouvez obtenir une adresse IP statique pour votre site web public.</span><span class="sxs-lookup"><span data-stu-id="3f572-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="3f572-110">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="3f572-110">Select **Save**.</span></span>

<span data-ttu-id="3f572-111">De plus, vous pouvez créer un enregistrement CNAME pour aider les clients à trouver votre site web.</span><span class="sxs-lookup"><span data-stu-id="3f572-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="3f572-112">Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="3f572-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="3f572-113">Pour **Type de DNS** entrez : **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="3f572-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="3f572-114">Pour **Nom d'hôte ou Alias**, tapez **www**</span><span class="sxs-lookup"><span data-stu-id="3f572-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="3f572-115">Pour **Adresse de pointage**, tapez le nom de domaine complet (FQDN) de votre site web (par exemple, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="3f572-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="3f572-116">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="3f572-116">Select **Save**.</span></span>
