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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815783"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Mettre à jour les enregistrements DNS pour conserver votre site web chez votre fournisseur d'hébergement actuel

1. Dans le centre d’administration 365 de Microsoft, accédez à la page domaines **d’installation**  >  [Domains](https://admin.microsoft.com/Adminportal#/Domains) , puis, dans la liste des domaines, sélectionnez le domaine que vous utilisez pour votre site Web.

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
