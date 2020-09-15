---
title: Modifier les serveurs de noms
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714686"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft

Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.
  
Pour configurer votre domaine dans Microsoft 365, les serveurs de noms de votre bureau d’enregistrement doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d’enregistrement de domaines.
  
1. Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.
  
2. Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Enregistrez les modifications.

Vous trouverez également des instructions détaillées dans cet article : [Modifier les serveurs de noms avec n’importe quel bureau d’enregistrement de domaines](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  