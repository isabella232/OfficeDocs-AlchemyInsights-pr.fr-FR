---
title: Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699517"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="4fc50-102">Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel</span><span class="sxs-lookup"><span data-stu-id="4fc50-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="4fc50-103">Dans le centre d’administration 365 de Microsoft, accédez à la page domaines **d’installation**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) , puis, dans la liste des domaines, sélectionnez le domaine que vous utilisez pour votre site Web.</span><span class="sxs-lookup"><span data-stu-id="4fc50-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="4fc50-104">Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="4fc50-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4fc50-105">Pour **Type de DNS** entrez : **A (Adresse)**</span><span class="sxs-lookup"><span data-stu-id="4fc50-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="4fc50-106">Pour **Nom d'hôte ou Alias**, tapez **@**.</span><span class="sxs-lookup"><span data-stu-id="4fc50-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="4fc50-107">Pour **Adresse IP**, tapez l'adresse IP statique correspondant à l'hébergement actuel de votre site web (par exemple, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="4fc50-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="4fc50-p101">Il doit s'agir d'une adresse IP  *statique*  pour le site web (et non d'une adresse IP  *dynamique*  ). Vérifiez l'emplacement d'hébergement de votre site web pour vous assurer que vous pouvez obtenir une adresse IP statique pour votre site web public.</span><span class="sxs-lookup"><span data-stu-id="4fc50-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="4fc50-110">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="4fc50-110">Select **Save**.</span></span>

<span data-ttu-id="4fc50-111">De plus, vous pouvez créer un enregistrement CNAME pour aider les clients à trouver votre site web.</span><span class="sxs-lookup"><span data-stu-id="4fc50-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="4fc50-112">Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="4fc50-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4fc50-113">Pour **Type de DNS** entrez : **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="4fc50-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="4fc50-114">Pour **Nom d'hôte ou Alias**, tapez **www**</span><span class="sxs-lookup"><span data-stu-id="4fc50-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="4fc50-115">Pour **Adresse de pointage**, tapez le nom de domaine complet (FQDN) de votre site web (par exemple, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4fc50-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="4fc50-116">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="4fc50-116">Select **Save**.</span></span>
