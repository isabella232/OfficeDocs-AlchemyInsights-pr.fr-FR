---
title: Teams autorise ou désactive la vidéo IP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826341"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="930fa-102">Teams autorise ou désactive la vidéo IP</span><span class="sxs-lookup"><span data-stu-id="930fa-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="930fa-103">**Modifier ou créer une stratégie de réunion**</span><span class="sxs-lookup"><span data-stu-id="930fa-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="930fa-104">Pour modifier ou créer une stratégie de réunion, accédez au **Centre d’administration Microsoft Teams > Réunions > Stratégies de réunion**.</span><span class="sxs-lookup"><span data-stu-id="930fa-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="930fa-105">Sélectionnez une stratégie dans la liste ou cliquez sur **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="930fa-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="930fa-106">Si vous créez une stratégie, ajoutez un nom et une description.</span><span class="sxs-lookup"><span data-stu-id="930fa-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="930fa-107">Le nom ne peut pas contenir de caractères spéciaux et ne doit pas dépasser 64 caractères.</span><span class="sxs-lookup"><span data-stu-id="930fa-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="930fa-108">Choisissez les paramètres, puis cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="930fa-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="930fa-109">Par exemple, imaginons que vous avez de nombreux d’utilisateurs et que vous voulez limiter la quantité de bande passante requise par la réunion.</span><span class="sxs-lookup"><span data-stu-id="930fa-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="930fa-110">Vous devez créer une stratégie personnalisée nommée « bande passante limitée » et désactiver les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="930fa-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="930fa-111">Sous **Audio & vidéo** :</span><span class="sxs-lookup"><span data-stu-id="930fa-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="930fa-112">Désactivez l’option Autoriser l’enregistrement Cloud.</span><span class="sxs-lookup"><span data-stu-id="930fa-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="930fa-113">Désactivez Autoriser la vidéo IP.</span><span class="sxs-lookup"><span data-stu-id="930fa-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="930fa-114">Vous pouvez ensuite attribuer la stratégie aux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="930fa-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="930fa-115">**Affecter une stratégie de réunion aux utilisateurs**</span><span class="sxs-lookup"><span data-stu-id="930fa-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="930fa-116">Dans le volet de navigation gauche du centre d’administration Microsoft Teams, et accédez aux **Utilisateurs**, puis cliquez sur l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="930fa-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="930fa-117">Sélectionnez l’utilisateur en cliquant à gauche du nom de celui-ci, puis cliquez sur **Modifier les paramètres**.</span><span class="sxs-lookup"><span data-stu-id="930fa-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="930fa-118">Sous **Stratégie de réunion**, sélectionnez la stratégie que vous souhaitez attribuer, et puis cliquez sur **Appliquer**.</span><span class="sxs-lookup"><span data-stu-id="930fa-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="930fa-119">Si vous souhaitez obtenir plus d’informations, voir [Gérer les stratégies de réunion dans Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="930fa-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
