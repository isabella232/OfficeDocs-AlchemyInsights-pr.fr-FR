---
title: Erreur de Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468939"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="2c8f8-102">Erreur Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="2c8f8-102">Winsock error 10061</span></span>

<span data-ttu-id="2c8f8-p101">Ce code d’erreur signifie que Office 365 n’a pas pu établir un socket TCP (connexion) avec l’hôte cible. La cause la plus probable de cette erreur est un problème avec votre configuration du pare-feu. Pour résoudre le problème, vérifiez ces paramètres :</span><span class="sxs-lookup"><span data-stu-id="2c8f8-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="2c8f8-106">Vérifiez votre configuration de pare-feu avec les informations contenues dans [Office 365 URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2c8f8-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="2c8f8-107">Si l’erreur est spécifique à Exchange Online Protection (EOP), vous devez ont été précédemment notifiés à une modification dans les [adresses IP de Protection Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2c8f8-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="2c8f8-108">Vérifiez que votre fournisseur de services Internet (Internet) n’est pas le blocage du port.</span><span class="sxs-lookup"><span data-stu-id="2c8f8-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="2c8f8-109">Vérifiez les paramètres du serveur hôte et cible actives dans vos connecteurs.</span><span class="sxs-lookup"><span data-stu-id="2c8f8-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="2c8f8-110">Notez que Office 365 ne bloque pas les connexions *entrantes* de cette manière.</span><span class="sxs-lookup"><span data-stu-id="2c8f8-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

