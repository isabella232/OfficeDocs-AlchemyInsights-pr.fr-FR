---
title: Envoi de la facturation par e-mail dans Azure moderne
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840600"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="2e908-102">Envoi de la facturation par e-mail dans Azure</span><span class="sxs-lookup"><span data-stu-id="2e908-102">Email invoicing in Azure</span></span>

<span data-ttu-id="2e908-103">Vous devez posséder le rôle de propriétaire ou de collaborateur sur le profil de facturation ou son compte de facturation pour mettre à jour ses préférences de facturation par e-mail.</span><span class="sxs-lookup"><span data-stu-id="2e908-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="2e908-104">Après activation, tous les utilisateurs disposant de rôles de propriétaire, de contributeur, de lecteur et de gestionnaire de factures dans un profil de facturation reçoivent la facture correspondante par e-mail.</span><span class="sxs-lookup"><span data-stu-id="2e908-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="2e908-105">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2e908-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="2e908-106">Recherchez **Gestion des coûts + Facturation**.</span><span class="sxs-lookup"><span data-stu-id="2e908-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="2e908-107">Sélectionnez **Factures** dans le côté gauche, puis **Facture par e-mail** en haut de la page.</span><span class="sxs-lookup"><span data-stu-id="2e908-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="2e908-108">Si vous possédez plusieurs profils de facturation, sélectionnez-en un, puis choisissez **Activation**.</span><span class="sxs-lookup"><span data-stu-id="2e908-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="2e908-109">Sélectionnez **Mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="2e908-109">Select **Update**.</span></span>
6. <span data-ttu-id="2e908-110">Si vous possédez plusieurs profils de facturation, sélectionnez-en un, puis choisissez **Activation**.</span><span class="sxs-lookup"><span data-stu-id="2e908-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="2e908-111">Vous autorisez d’autres personnes à afficher, télécharger et régler les factures en leur attribuant le rôle de gestionnaire de factures pour un profil de facturation MCA ou MPA.</span><span class="sxs-lookup"><span data-stu-id="2e908-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="2e908-112">Si vous avez activé l’envoi des factures par e-mail, les utilisateurs reçoivent également les factures par e-mail.</span><span class="sxs-lookup"><span data-stu-id="2e908-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="2e908-113">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2e908-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="2e908-114">Recherchez **Gestion des coûts + Facturation**.</span><span class="sxs-lookup"><span data-stu-id="2e908-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="2e908-115">Sélectionnez **Profils de facturation** dans le côté gauche.</span><span class="sxs-lookup"><span data-stu-id="2e908-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="2e908-116">Dans la liste des profils de facturation, sélectionnez celui auquel vous voulez attribuer un rôle de gestionnaire de factures.</span><span class="sxs-lookup"><span data-stu-id="2e908-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="2e908-117">Sélectionnez **Contrôle d’accès (IAM)** dans le côté gauche, puis **Ajouter** en haut de la page.</span><span class="sxs-lookup"><span data-stu-id="2e908-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="2e908-118">Dans la liste déroulante Rôle, sélectionnez **Gestionnaire de factures**.</span><span class="sxs-lookup"><span data-stu-id="2e908-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="2e908-119">Entrez l’adresse e-mail de l’utilisateur pour lui donner accès.</span><span class="sxs-lookup"><span data-stu-id="2e908-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="2e908-120">Sélectionnez **Enregistrer** pour attribuer le rôle.</span><span class="sxs-lookup"><span data-stu-id="2e908-120">Select **Save** to assign the role.</span></span>
