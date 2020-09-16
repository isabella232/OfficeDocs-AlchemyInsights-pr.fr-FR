---
title: Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734909"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft

Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.
  
Pour configurer votre domaine avec Microsoft, les serveurs de noms de votre serveur d’inscriptions doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d'enregistrement de domaine.
  
1. Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.

2. Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Enregistrez les modifications.

Vous trouverez également des instructions détaillées dans cet article : [modifier les serveurs de noms pour configurer Microsoft 365 avec n’importe quel bureau](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) d’enregistrement de domaines
  