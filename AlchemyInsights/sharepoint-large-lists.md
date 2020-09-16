---
title: Grandes listes SharePoint
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
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720131"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="6c652-102">Utiliser des listes et des bibliothèques volumineuses dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="6c652-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="6c652-103">Les listes et bibliothèques SharePoint peuvent contenir jusqu’à 30 millions éléments, mais lorsqu’ils ont plus de 5 000 éléments, vous pouvez voir une erreur de seuil d’affichage de liste lorsque vous essayez de les utiliser.</span><span class="sxs-lookup"><span data-stu-id="6c652-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="6c652-104">Ce seuil a pour but de maintenir les performances du service.</span><span class="sxs-lookup"><span data-stu-id="6c652-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="6c652-105">Il n’est pas possible de le modifier.</span><span class="sxs-lookup"><span data-stu-id="6c652-105">It can't be changed.</span></span> <span data-ttu-id="6c652-106">Pour éviter d’atteindre ce seuil, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6c652-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="6c652-107">**Utiliser moderne**</span><span class="sxs-lookup"><span data-stu-id="6c652-107">**Use modern**</span></span>

<span data-ttu-id="6c652-108">Les affichages présentant un grand nombre d’éléments fonctionnent mieux dans l’expérience moderne.</span><span class="sxs-lookup"><span data-stu-id="6c652-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="6c652-109">[Utilisez l’expérience moderne](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) pour éviter les erreurs que vous pouvez voir dans l’expérience classique.</span><span class="sxs-lookup"><span data-stu-id="6c652-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="6c652-110">**Ajouter des index**</span><span class="sxs-lookup"><span data-stu-id="6c652-110">**Add indexes**</span></span>

<span data-ttu-id="6c652-111">Lorsque vous filtrez ou triez sur une colonne qui n’a pas d’index, un message d’erreur peut s’afficher.</span><span class="sxs-lookup"><span data-stu-id="6c652-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="6c652-112">[Ajoutez un index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellement à partir des paramètres de la **liste** dans le menu paramètres, puis dans les **colonnes indexées**.</span><span class="sxs-lookup"><span data-stu-id="6c652-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="6c652-113">**Modifier l’affichage de liste**</span><span class="sxs-lookup"><span data-stu-id="6c652-113">**Edit the list view**</span></span>

<span data-ttu-id="6c652-114">Si une erreur se produit lorsque vous travaillez dans une grande liste, [Modifiez votre vue de liste](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="6c652-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="6c652-115">Les quatre modifications suivantes suppriment les erreurs de seuil d’affichage de liste.</span><span class="sxs-lookup"><span data-stu-id="6c652-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="6c652-116">Pour supprimer toutes les erreurs, effectuez les quatre modifications.</span><span class="sxs-lookup"><span data-stu-id="6c652-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="6c652-117">Si vous obtenez toujours des erreurs, cochez [gérer les grandes listes et les bibliothèques](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="6c652-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="6c652-118">Sélectionnez **aucun** dans **le premier tri par la colonne** , **puis triez par la colonne**.</span><span class="sxs-lookup"><span data-stu-id="6c652-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="6c652-119">Sélectionnez **aucun** dans **le premier groupe par la colonne** , puis **regrouper sur la colonne**.</span><span class="sxs-lookup"><span data-stu-id="6c652-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="6c652-120">Sélectionnez **aucun** pour toutes les colonnes de la section **totaux** .</span><span class="sxs-lookup"><span data-stu-id="6c652-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="6c652-121">Désélectionnez toutes les colonnes sauf une pour l’affichage dans la section **colonnes** .</span><span class="sxs-lookup"><span data-stu-id="6c652-121">Deselect all but one column for display from the **Columns** section.</span></span>

