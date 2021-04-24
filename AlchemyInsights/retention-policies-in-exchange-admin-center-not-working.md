---
title: Les stratégies de rétention dans le Centre d'administration Exchange ne fonctionnent pas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952226"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1cd4b-102">Stratégies de rétention dans le Centre d'administration Exchange</span><span class="sxs-lookup"><span data-stu-id="1cd4b-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="1cd4b-103">Si vous souhaitez que nous 2007-2016 exécutez des vérifications automatisées pour les paramètres mentionnés ci-dessous, sélectionnez le bouton Retour <- en haut de cette page, puis entrez l'adresse e-mail de l'utilisateur qui a des problèmes avec les stratégies de rétention.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="1cd4b-104">Si vous avez des problèmes avec les stratégies de rétention dans le Centre d'administration Exchange qui ne s'appliquent pas aux boîtes aux lettres ou aux éléments qui ne sont pas en déplacement vers la boîte aux lettres d'archivage, vérifiez les points suivants :</span><span class="sxs-lookup"><span data-stu-id="1cd4b-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="1cd4b-105">**Causes premières :**</span><span class="sxs-lookup"><span data-stu-id="1cd4b-105">**Root Causes:**</span></span>

- <span data-ttu-id="1cd4b-106">**L'Assistant Dossier géré** n'a pas traitée la boîte aux lettres de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="1cd4b-107">L'Assistant Dossier géré tente de traiter toutes les boîtes aux lettres de votre organisation en nuage tous les sept jours.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="1cd4b-108">**Solution :** Exécutez l'Assistant Dossier géré.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="1cd4b-109">**RetentionHold** a été **activé sur la** boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="1cd4b-110">Si la boîte aux lettres a été placée sur un retentionHold, la stratégie de rétention sur la boîte aux lettres n'est pas traitée pendant cette période.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="1cd4b-111">**Solution :** Vérifiez l'état du paramètre conservation de rétention et mettez-le à jour selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="1cd4b-112">Pour plus d'informations, voir [Conservation de rétention de boîte aux lettres.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="1cd4b-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="1cd4b-113">**Remarque :** Si une boîte aux lettres est plus petite que 10 Mo, l'Assistant Dossier géré ne traitera pas automatiquement la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1cd4b-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="1cd4b-114">Pour plus d'informations sur les stratégies de rétention dans le Centre d'administration Exchange, voir :</span><span class="sxs-lookup"><span data-stu-id="1cd4b-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="1cd4b-115">Balises et stratégies de rétention</span><span class="sxs-lookup"><span data-stu-id="1cd4b-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="1cd4b-116">[Appliquer une stratégie de rétention à des boîtes aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou ajouter ou supprimer des [balises de rétention](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="1cd4b-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="1cd4b-117">Comment identifier le type de conservation placé sur une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="1cd4b-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
