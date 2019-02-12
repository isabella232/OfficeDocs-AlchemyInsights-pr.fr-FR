---
title: Erreur de Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903095"
---
# <a name="winsock-error-10061"></a>Erreur Winsock 10061

Ce code d’erreur signifie que Office 365 n’a pas pu établir un socket TCP (connexion) avec l’hôte cible. La cause la plus probable de cette erreur est un problème avec votre configuration du pare-feu. Pour résoudre le problème, vérifiez ces paramètres :
  
- Vérifiez votre configuration de pare-feu avec les informations contenues dans [Office 365 URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Si l’erreur est spécifique à Exchange Online Protection (EOP), vous devez ont été précédemment notifiés à une modification dans les [adresses IP de Protection Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Vérifiez que votre fournisseur de services Internet (Internet) n’est pas le blocage du port.
    
- Vérifiez les paramètres du serveur hôte et cible actives dans vos connecteurs.
    
Notez que Office 365 ne bloque pas les connexions *entrantes* de cette manière. 
  

