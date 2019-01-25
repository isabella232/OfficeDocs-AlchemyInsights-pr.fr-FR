---
title: Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468812"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="57fed-102">Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel</span><span class="sxs-lookup"><span data-stu-id="57fed-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="57fed-103">Sur la page [Domaines](https://portal.office.com/adminportal/home#/Domains), dans la liste de domaines, cliquez sur celui que vous utilisez pour votre site web, puis sélectionnez **Paramètres DNS** dans le volet de gestion.</span><span class="sxs-lookup"><span data-stu-id="57fed-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="57fed-104">Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="57fed-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="57fed-105">Pour **Type de DNS** entrez : **A (Adresse)**</span><span class="sxs-lookup"><span data-stu-id="57fed-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="57fed-106">Pour **Nom d'hôte ou Alias**, tapez **@**.</span><span class="sxs-lookup"><span data-stu-id="57fed-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="57fed-107">Pour **Adresse IP**, tapez l'adresse IP statique correspondant à l'hébergement actuel de votre site web (par exemple, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="57fed-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="57fed-p101">Il doit s'agir d'une adresse IP  *statique*  pour le site web (et non d'une adresse IP  *dynamique*  ). Vérifiez l'emplacement d'hébergement de votre site web pour vous assurer que vous pouvez obtenir une adresse IP statique pour votre site web public.</span><span class="sxs-lookup"><span data-stu-id="57fed-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="57fed-110">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="57fed-110">Select **Save**.</span></span> 
    
<span data-ttu-id="57fed-111">De plus, vous pouvez créer un enregistrement CNAME pour aider les clients à trouver votre site web.</span><span class="sxs-lookup"><span data-stu-id="57fed-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="57fed-112">Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="57fed-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="57fed-113">Pour **Type de DNS** entrez : **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="57fed-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="57fed-114">Pour **Nom d'hôte ou Alias**, tapez **www**</span><span class="sxs-lookup"><span data-stu-id="57fed-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="57fed-115">Pour **Adresse de pointage**, tapez le nom de domaine complet (FQDN) de votre site web (par exemple, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="57fed-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="57fed-116">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="57fed-116">Select **Save**.</span></span> 
    

