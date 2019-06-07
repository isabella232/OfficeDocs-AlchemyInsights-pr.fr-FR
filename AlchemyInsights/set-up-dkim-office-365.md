---
title: Configurer DKIM dans Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765055"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="c3b31-102">Configurer DKIM dans Office 365</span><span class="sxs-lookup"><span data-stu-id="c3b31-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="c3b31-103">[Voici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)les instructions complètes de configuration de DKIM pour les domaines personnalisés dans Office 365.</span><span class="sxs-lookup"><span data-stu-id="c3b31-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="c3b31-104">Pour **chaque** domaine personnalisé, vous devez créer **deux** enregistrements CNAME DKIM au niveau du service d’hébergement DNS de votre domaine (généralement, le Bureau d’enregistrement de domaines).</span><span class="sxs-lookup"><span data-stu-id="c3b31-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="c3b31-105">Par exemple, contoso.com et fourthcoffee.com requièrent quatre enregistrements CNAMe DKIM: deux pour contoso.com et deux pour fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="c3b31-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="c3b31-106">Les enregistrements CNAMe DKIM pour **chaque** domaine personnalisé utilisent les formats suivants:</span><span class="sxs-lookup"><span data-stu-id="c3b31-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="c3b31-107">**Nom**de l’hôte:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="c3b31-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="c3b31-108">**Pointe vers l’adresse ou la valeur**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="c3b31-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="c3b31-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="c3b31-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="c3b31-110">**Nom**de l’hôte:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="c3b31-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="c3b31-111">**Pointe vers l’adresse ou la valeur**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="c3b31-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="c3b31-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="c3b31-112">**TTL**: 3600</span></span>

   <span data-ttu-id="c3b31-113">\<DomainGUID\> est le texte à gauche de `.mail.protection.outlook.com` dans l’enregistrement MX personnalisé pour le domaine personnalisé (par exemple, `contoso-com` pour le domaine contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c3b31-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="c3b31-114">\<InitialDomain\> est le domaine que vous avez utilisé lorsque vous vous êtes inscrit à Office 365 (par exemple, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="c3b31-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="c3b31-115">Une fois que vous avez créé les enregistrements CNAMe pour vos domaines personnalisés, procédez comme suit:</span><span class="sxs-lookup"><span data-stu-id="c3b31-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="c3b31-116">a.</span><span class="sxs-lookup"><span data-stu-id="c3b31-116">a.</span></span> <span data-ttu-id="c3b31-117">[Connectez-vous à Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) à l'aide de votre compte professionnel ou scolaire.</span><span class="sxs-lookup"><span data-stu-id="c3b31-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="c3b31-118">b.</span><span class="sxs-lookup"><span data-stu-id="c3b31-118">b.</span></span> <span data-ttu-id="c3b31-119">Sélectionnez l’icône du lanceur d’applications située en haut à gauche et choisissez **Administrateur**.</span><span class="sxs-lookup"><span data-stu-id="c3b31-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="c3b31-120">c.</span><span class="sxs-lookup"><span data-stu-id="c3b31-120">c.</span></span> <span data-ttu-id="c3b31-121">Dans le volet de navigation en bas à gauche, développez **Administrateur** et choisissez **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c3b31-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="c3b31-122">d.</span><span class="sxs-lookup"><span data-stu-id="c3b31-122">d.</span></span> <span data-ttu-id="c3b31-123">Accédez à **protection** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="c3b31-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="c3b31-124">e.</span><span class="sxs-lookup"><span data-stu-id="c3b31-124">e.</span></span> <span data-ttu-id="c3b31-125">Sélectionnez le domaine, puis sélectionnez **activer** pour **signer les messages pour ce domaine avec des signatures DKIM**.</span><span class="sxs-lookup"><span data-stu-id="c3b31-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="c3b31-126">Répétez cette étape pour chaque domaine personnalisé.</span><span class="sxs-lookup"><span data-stu-id="c3b31-126">Repeat this step for each custom domain.</span></span>
