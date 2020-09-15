---
title: Erreurs de création d’événements en direct dans Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675440"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="0f703-102">Erreurs de création d’événements en direct dans Yammer</span><span class="sxs-lookup"><span data-stu-id="0f703-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="0f703-103">**Création d’un événement en direct dans Yammer**</span><span class="sxs-lookup"><span data-stu-id="0f703-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="0f703-104">Yammer affiche à tout moment l’option de création d’un événement en direct.</span><span class="sxs-lookup"><span data-stu-id="0f703-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="0f703-105">Dans certains cas, un utilisateur ne répond peut-être pas aux conditions préalables à la création d’un événement en direct et reçoit un message d’erreur lorsqu’il tente de le créer.</span><span class="sxs-lookup"><span data-stu-id="0f703-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="0f703-106">Les éléments ci-dessous décrivent les raisons habituelles de ce problème et offrent des solutions pour le résoudre chez les utilisateurs finaux.</span><span class="sxs-lookup"><span data-stu-id="0f703-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="0f703-107">**Qui peut créer un événement en direct ?**</span><span class="sxs-lookup"><span data-stu-id="0f703-107">**Who can create live events**</span></span>
- <span data-ttu-id="0f703-108">Une licence Office 365 Entreprise E1, E3 ou E5, ou une licence Office 365 A3 ou A5.</span><span class="sxs-lookup"><span data-stu-id="0f703-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="0f703-109">L’autorisation de créer des événements en direct dans le centre d’administration Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0f703-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="0f703-110">L’autorisation de créer des événements en direct dans Microsoft Stream (pour les événements générés à l’aide d’une application ou d’un appareil de diffusion externe).</span><span class="sxs-lookup"><span data-stu-id="0f703-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="0f703-111">Appartenance totale à une équipe au sein de l’organisation (vous ne pouvez pas être un invité ou une autre organisation).</span><span class="sxs-lookup"><span data-stu-id="0f703-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="0f703-112">Planification des réunions privées, ainsi que partage d’écran et de vidéos IP, activés dans la stratégie de réunion d’équipe.</span><span class="sxs-lookup"><span data-stu-id="0f703-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="0f703-113">**Stratégies de création d’événements en direct**</span><span class="sxs-lookup"><span data-stu-id="0f703-113">**Live event creation policies**</span></span>

<span data-ttu-id="0f703-114">Yammer suit les stratégies d’événement en direct définies chez votre client Office 365 pour Stream.</span><span class="sxs-lookup"><span data-stu-id="0f703-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="0f703-115">Par défaut, tous les membres de votre organisation peuvent créer des événements en direct.</span><span class="sxs-lookup"><span data-stu-id="0f703-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="0f703-116">Les administrateurs peuvent [modifier ce paramètre, ce qui peut empêcher les utilisateurs de créer un événement en direct](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="0f703-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="0f703-117">Il est important de vérifier que les utilisateurs disposent des autorisations nécessaires pour créer des événements en direct s’ils reçoivent une erreur de stratégie.</span><span class="sxs-lookup"><span data-stu-id="0f703-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
