---
title: Workday pour l’approvisionnement des utilisateurs AD passe en état de mise en quarantaine
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430744"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="0c0ff-102">Workday pour l’approvisionnement des utilisateurs AD passe en état de mise en quarantaine</span><span class="sxs-lookup"><span data-stu-id="0c0ff-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="0c0ff-103">**Workday pour l’approvisionnement des utilisateurs AD passe en état de mise en quarantaine et aucun utilisateur n'est créé dans AD**</span><span class="sxs-lookup"><span data-stu-id="0c0ff-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="0c0ff-104">La tâche Workday pour l’approvisionnement des utilisateurs AD est passée à l’état de mise en quarantaine et les journaux d’audit affichent des événements d’échec de l’exportation avec le message d’erreur **Erreur :OperationsError-SvcErr : une erreur d’opération s’est produite. Aucune référence supérieure n’a été configurée pour le service de répertoire. Le service de répertoire est donc incapable d’émettre des références aux objets en dehors de cette forêt**.</span><span class="sxs-lookup"><span data-stu-id="0c0ff-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="0c0ff-105">Cette erreur s’affiche généralement si le conteneur Active Directory OU n’est pas configuré correctement ou s’il existe des problèmes avec le Mappage d’expression utilisé pour **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="0c0ff-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="0c0ff-106">Recherchez des fautes de frappe dans la valeur par défaut OU for le paramètre **Nouveaux utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="0c0ff-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="0c0ff-107">Veillez à ce que le conteneur OU spécifié existe déjà dans votre AD.</span><span class="sxs-lookup"><span data-stu-id="0c0ff-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="0c0ff-108">Si vous utilisez **parentDistinguishedName** dans le mappage d’attribut, veillez à ce qu’il s’évalue toujours au conteneur connu dans le domaine AD.</span><span class="sxs-lookup"><span data-stu-id="0c0ff-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="0c0ff-109">Recherchez l’événement Exportation dans les journaux d’audit pour afficher la valeur générée.</span><span class="sxs-lookup"><span data-stu-id="0c0ff-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="0c0ff-110">Pour d’autres détails sur la configuration de Workday pour l’approvisionnement automatique, voir [Tutoriel : Configurer Workday pour l'approvisionnement automatique d'utilisateurs](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="0c0ff-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

