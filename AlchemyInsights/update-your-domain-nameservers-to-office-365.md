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
ms.openlocfilehash: d9d66e366db14840a86b681deba78b89ddff5e068a3b931c88e493d2ec791b10
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073598"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft

Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.
  
Pour configurer votre domaine auprès de Microsoft, les serveurs de noms de votre bureau d’enregistrement doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d'enregistrement de domaine.
  
1. Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.

2. Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Enregistrez les modifications.

Vous trouverez également des instructions détaillées dans cet article : Modifier les serveurs de noms pour configurer Microsoft 365 auprès d’un bureau d’enregistrement [de domaines](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  