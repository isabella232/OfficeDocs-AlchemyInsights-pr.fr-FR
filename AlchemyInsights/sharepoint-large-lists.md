---
title: SharePoint grandes listes
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941587"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Travailler avec des listes et des bibliothèques de grande taille dans SharePoint

SharePoint listes et bibliothèques peuvent contenir jusqu’à 30 millions d’éléments, mais lorsqu’elles contiennent plus de 5 000 éléments, une erreur de seuil d’affichage de liste peut s’afficher lorsque vous essayez de les utiliser. Ce seuil a pour but de maintenir les performances du service. Il n’est pas possible de le modifier. Pour éviter d’atteindre ce seuil :

**Utiliser moderne**

Les affichages montrant de nombreux éléments fonctionnent mieux dans l’expérience moderne. [Utilisez l’expérience moderne pour](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) éviter les erreurs que vous pouvez voir dans l’expérience classique.

**Ajouter des index**

Lorsque vous filtrez ou tiez par colonne qui ne comprend pas d’index, vous pouvez voir un message d’erreur. [Ajoutez manuellement un index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) à **partir Paramètres** liste dans le menu Paramètres, puis **colonnes indexées**.

**Modifier l’affichage liste**

Si une erreur se produit lorsque vous travaillez avec une grande liste, [modifiez votre affichage de liste.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)

Les quatre modifications suivantes suppriment les erreurs de seuil d’affichage de liste. A effectuer les quatre modifications pour supprimer toutes les erreurs. Si vous continuez à recevoir des erreurs, vérifiez [Gérer les grandes listes et bibliothèques.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Sélectionnez **Aucun** dans **le premier tri par colonne,** puis tri par **colonne.**
2. Sélectionnez **Aucun** dans le **premier groupe par colonne et** puis par **colonne.**
3. Sélectionnez **Aucun** pour toutes les colonnes de la section **Totaux.**
4. Désélectionner toutes les colonnes à afficher à partir de la section **Colonnes.**

