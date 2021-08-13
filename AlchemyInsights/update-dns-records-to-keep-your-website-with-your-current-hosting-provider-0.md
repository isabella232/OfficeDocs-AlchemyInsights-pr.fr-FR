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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007680"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel

1. Dans la Centre d’administration Microsoft 365, allez à la page Domaines  >  [](https://admin.microsoft.com/Adminportal#/Domains) d’installation et, dans la liste des domaines, sélectionnez le domaine que vous utilisez pour votre site web.

2. Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :

  - Pour **Type de DNS** entrez : **A (Adresse)**

  - Pour **Nom d'hôte ou Alias**, tapez **@**.

  - Pour **Adresse IP**, tapez l'adresse IP statique correspondant à l'hébergement actuel de votre site web (par exemple, 172.16.140.1).

    Il doit s'agir d'une adresse IP  *statique*  pour le site web (et non d'une adresse IP  *dynamique*  ). Vérifiez l'emplacement d'hébergement de votre site web pour vous assurer que vous pouvez obtenir une adresse IP statique pour votre site web public.

3. Sélectionnez **Enregistrer**.

De plus, vous pouvez créer un enregistrement CNAME pour aider les clients à trouver votre site web.
  
1. Sélectionnez **+Nouvel enregistrement personnalisé** et entrez les éléments suivants :

  - Pour **Type de DNS** entrez : **CNAME (Alias)**

  - Pour **Nom d'hôte ou Alias**, tapez **www**

  - Pour **Adresse de pointage**, tapez le nom de domaine complet (FQDN) de votre site web (par exemple, contoso.com).

2. Sélectionnez **Enregistrer**.
