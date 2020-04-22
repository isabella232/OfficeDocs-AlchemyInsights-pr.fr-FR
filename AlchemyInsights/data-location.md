---
title: Emplacement des données
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655280"
---
# <a name="data-location"></a>Emplacement des données

Vous pouvez afficher l’emplacement de votre client dans le centre d’administration ou en vous connectant à Exchange Online via PowerShell.


**Centre d’administration :**
1. Connectez-vous au [Centre d’administration](https://admin.microsoft.com/Adminportal/Home).
2. Sélectionnez **Settings** > **profil d’organisation**des paramètres.
3. Sous **emplacement des données**, sélectionnez **afficher les détails**.


**PowerShell**
1. Connectez-vous à Exchange Online à l’aide de Windows PowerShell.
2. Exécutez la cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) pour afficher la liste des propriétés de votre client. 
3. Examinez la propriété PageY.

Lorsque vous disposez de l’emplacement des données pour EXO et SPO, vous pouvez déterminer l’emplacement des données pour les autres services que vous pouvez utiliser à l' [endroit où se trouvent vos données](https://products.office.com/where-is-your-data-located).