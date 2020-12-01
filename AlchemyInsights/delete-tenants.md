---
title: Supprimer un locataire
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477677"
---
# <a name="delete-tenant"></a><span data-ttu-id="2ffcd-102">Supprimer un locataire</span><span class="sxs-lookup"><span data-stu-id="2ffcd-102">Delete tenant</span></span>

<span data-ttu-id="2ffcd-103">Pour supprimer un Azure AD, vérifiez les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="2ffcd-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="2ffcd-104">Vous êtes un administrateur général de l’annuaire.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="2ffcd-105">Vous n’êtes pas connecté avec un compte qui a le répertoire par défaut tel que contoso.onmicrosoft.com dans le compte connecté, tel que admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="2ffcd-106">Supprimez toutes les applications actives dans l’annuaire avant la suppression.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="2ffcd-107">Pour supprimer des applications actives, accédez à inscriptions des applications et supprimez les applications existantes.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="2ffcd-108">Il n’existe aucun abonnement actif pour Microsoft Online Services, tel que Microsoft Azure, Office 365 ou Azure AD Premium associé à l’annuaire.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="2ffcd-109">Transférez vos abonnements ou Accélérez l’annulation des abonnements actifs via la prise en charge et la facturation Azure.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="2ffcd-110">Pour en savoir plus, consultez la procédure d’annulation des abonnements Office 365 et Azure.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="2ffcd-111">Pour obtenir des instructions sur l’Association ou l’ajout d’un abonnement existant à un client, reportez-vous à [la rubrique associer ou ajouter un abonnement Azure à votre client Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="2ffcd-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="2ffcd-112">Il n’y a pas de licence active.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-112">There are no Active license.</span></span> <span data-ttu-id="2ffcd-113">Pour supprimer des licences, consultez [la rubrique How to Remove Subscription to Remove License](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="2ffcd-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="2ffcd-114">Il n’y a pas d’autres utilisateurs actifs dans l’annuaire, outre vous-même en tant qu’administrateur général lors de la tentative de suppression d’Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="2ffcd-115">Supprimez tous les autres utilisateurs actifs, et toutes les dépendances d’un nom de domaine personnalisé dans le client doivent également être supprimées, telles que les utilisateurs créés avec admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="2ffcd-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="2ffcd-116">Pour plus d’informations sur la procédure :</span><span class="sxs-lookup"><span data-stu-id="2ffcd-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="2ffcd-117">Supprimez « Azure Active Directory » ou « abonnement », consultez la rubrique [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="2ffcd-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="2ffcd-118">Suppression d’applications dans l’annuaire, consultez la rubrique [Suppression d’applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="2ffcd-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
