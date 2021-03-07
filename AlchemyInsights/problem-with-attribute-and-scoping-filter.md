---
title: Problème avec l’attribut et le filtre d’étendue
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430750"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="3fbfa-102">Problème avec l’attribut et le filtre d’étendue</span><span class="sxs-lookup"><span data-stu-id="3fbfa-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="3fbfa-103">**Problème avec les valeurs UPN conflictuelles**</span><span class="sxs-lookup"><span data-stu-id="3fbfa-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="3fbfa-104">Le Workday pour l’approvisionnement d’utilisateurs AD affiche le message d’erreur **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="3fbfa-105">L’opération a échoué car la valeur UPN fournie pour l’ajout/modification n’est pas unique à l’échelle de la forêt.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="3fbfa-106">Détails de l’erreur : **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="3fbfa-107">La valeur **userPrincipalName** que le connecteur Workday tente de définir lors de la création du compte utilisateur AD existe déjà dans le domaine AD cible.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="3fbfa-108">Ceci implique que (1) l’utilisateur existe déjà et la vérification d’ID correspondante a échoué pour l’utilisateur ou (2) la règle de génération UPN a créé une valeur en conflit.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="3fbfa-109">Voici les étapes de résolution suggérées :</span><span class="sxs-lookup"><span data-stu-id="3fbfa-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="3fbfa-110">Si l’utilisateur existe déjà et que l’ID correspondante n’a pas pu lier le compte Workday au compte Active Directory, vérifiez alors si l’attribut d’ID correspondant (généralement **employeeID**) dans Workday et AD correspond exactement.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="3fbfa-111">S’il n’existe pas de correspondance, il s’agit d’un problème nécessitant une correction.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="3fbfa-112">Par exemple, si l’EmployeeID est 001052 dans Workday et 1052 dans AD, le moteur d’approvisionnement ne pourra alors pas lier les deux comptes et tentera de créer un utilisateur qui existe déjà.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="3fbfa-113">La solution dans ce cas est de modifier la valeur **EmployeeID** dans AD pour inclure les zéros du début afin qu’elle soit 001052.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="3fbfa-114">Si l’expression générant l’UPN ne créée pas de valeur unique, envisagez d’utiliser la fonction de déduplication **SelectUniqueValue** pour générer une valeur unique à chaque fois.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="3fbfa-115">**Workday pour l’approvisionnement d’utilisateurs AD ne définit pas la valeur d’attribut manager pour le compte des utilisateurs AD**</span><span class="sxs-lookup"><span data-stu-id="3fbfa-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="3fbfa-116">La tâche Workday pour l’approvisionnement d’utilisateurs AD ne définit pas la valeur d’attribut **manager** pour les comptes des utilisateurs AD.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="3fbfa-117">Il existe deux scénarios possibles lorsque vous voyez ce comportement :</span><span class="sxs-lookup"><span data-stu-id="3fbfa-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="3fbfa-118">Le manager dans Workday ne peut pas être résolu dans un compte d’utilisateur AD correspondant car le manager ne se trouve pas dans l’étendue.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="3fbfa-119">Dans un scénario de **domaines AD multiples**, le manager dans Workday n’est pas présent dans le même domaine que celui de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="3fbfa-120">Pour résoudre le problème, essayez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="3fbfa-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="3fbfa-121">Si vous avez défini des filtres d’étendue, vérifiez d’abord que le manager est dans l’étendue et qu’il satisfait la clause d’étendue.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="3fbfa-122">Si le manager ne satisfait pas le filtre d’étendue, modifiez le filtre, de sorte que le manage se trouve également dans l’étendue de l’opération d’approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="3fbfa-123">Si vous disposez de domaines AD multiples, le connecteur a donc une limitation connue d’incapacité à résoudre les références manager inter-domaines.</span><span class="sxs-lookup"><span data-stu-id="3fbfa-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="3fbfa-124">Pour d’autres détails sur la configuration de Workday pour l’approvisionnement automatique, voir [Tutoriel : Configurer Workday pour l'approvisionnement automatique d'utilisateurs](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="3fbfa-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













