---
title: 1554 erreur Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766167"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="674b0-102">Erreur Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="674b0-102">Winsock error 10061</span></span>

<span data-ttu-id="674b0-103">Ce code d’erreur signifie que Microsoft n’a pas pu établir un socket TCP (connexion) avec l’hôte cible.</span><span class="sxs-lookup"><span data-stu-id="674b0-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="674b0-104">La cause la plus probable de cette erreur est un problème avec la configuration de votre pare-feu.</span><span class="sxs-lookup"><span data-stu-id="674b0-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="674b0-105">Pour résoudre le problème, vérifiez les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="674b0-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="674b0-106">Vérifier la configuration de votre pare-feu avec les informations contenues dans les [URL et plages d’adresses IP de Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="674b0-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="674b0-107">Si l’erreur est spécifique à Exchange Online Protection (EOP), vous devriez avoir été préalablement notifié à une modification apportée aux [adresses IP d’Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="674b0-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="674b0-108">Vérifiez que votre fournisseur de services Internet (ISP) ne bloque pas le port.</span><span class="sxs-lookup"><span data-stu-id="674b0-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="674b0-109">Vérifiez les paramètres de l’hôte actif et du serveur cible dans vos connecteurs.</span><span class="sxs-lookup"><span data-stu-id="674b0-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="674b0-110">Notez que Microsoft 365 ne bloque pas les connexions *entrantes* de cette manière.</span><span class="sxs-lookup"><span data-stu-id="674b0-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
