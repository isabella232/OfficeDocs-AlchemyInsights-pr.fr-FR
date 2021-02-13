---
title: Gérer une identité managée affectée par l’utilisateur
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177302"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="e9873-102">Gérer une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="e9873-103">La gestion d’une identité managée affectée par l’utilisateur comprend les actions suivantes :</span><span class="sxs-lookup"><span data-stu-id="e9873-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="e9873-104">Affectation de rôles à une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="e9873-105">Suppression d’une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="e9873-106">Référencement d’une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="e9873-107">Si vous souhaitez en savoir plus d'informations sur les tâches mentionnées ci-dessus, veuillez consulter les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="e9873-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="e9873-108">[Créer une identité managée affectée par l’utilisateur](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) : pour l’attribution de rôles à une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="e9873-109">[Supprimer une identité managée affectée par l’utilisateur](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) : pour supprimer une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="e9873-110">[Répertorier une identité managée affectée par l’utilisateur](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) : pour répertorier une identité managée affectée par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e9873-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="e9873-111">Vérifiez si vous avez le rôle de **collaborateur d’identité gérée**.</span><span class="sxs-lookup"><span data-stu-id="e9873-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="e9873-112">Cette affectation de rôle est obligatoire pour créer/supprimer des identités gérées par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e9873-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
