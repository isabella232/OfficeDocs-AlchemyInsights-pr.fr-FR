---
title: Problème avec un seul utilisateur
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428689"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="540de-102">Problème avec un seul utilisateur</span><span class="sxs-lookup"><span data-stu-id="540de-102">Problem with single user</span></span>

- <span data-ttu-id="540de-103">L’utilisateur n’a peut-être pas été mis en service car le service n’a pas encore eu l’occasion d’évaluer l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="540de-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="540de-104">Examinez les instructions pour la durée de l’approvisionnement, ainsi que la barre de progression sur la page de configuration de l’approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="540de-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="540de-105">Si l’état stable spécifié dans la section détails supplémentaires se trouve avant la date de création/mise à jour/suppression de l’utilisateur, cela signifie que nous n’avons pas encore évalué l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="540de-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="540de-106">Dans ce scénario, la meilleure chose à faire est d’attendre la fin du service d’approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="540de-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="540de-107">Notez que notre service ne connaît que les modifications apportées à un utilisateur dans le système source (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="540de-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="540de-108">Il doit y avoir une modification valide dans le système source pour Azure AD afin de détecter la modification et de la faire circuler dans Active Directory.</span><span class="sxs-lookup"><span data-stu-id="540de-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="540de-109">Le service d’approvisionnement a évalué l’utilisateur et déterminé qu’il ne doit pas l’être :</span><span class="sxs-lookup"><span data-stu-id="540de-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="540de-110">Si vous avez définis un filtre d’attribution d’une portée basée sur les attributs, assurez-vous que l’utilisateur répond aux critères que vous avez spécifiés.</span><span class="sxs-lookup"><span data-stu-id="540de-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="540de-111">Si des utilisateurs existent déjà dans le système cible et l’état de l’utilisateur dans la correspondance source et cible, nous n’allons pas prendre d’autres mesures.</span><span class="sxs-lookup"><span data-stu-id="540de-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="540de-112">Le service d’approvisionnement a tenté de mettre en service l’utilisateur et a échoué.</span><span class="sxs-lookup"><span data-stu-id="540de-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="540de-113">Pour ces scénarios, examinez l’onglet Résolution des problèmes et recommandations des journaux d’approvisionnement :</span><span class="sxs-lookup"><span data-stu-id="540de-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="540de-114">Un attribut requis sur l’utilisateur peut être manquant dans Active Directory local ou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="540de-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="540de-115">Par exemple, les règles de génération userPrincipalName ou sAMAccountName ne génèrent pas la bonne valeur.</span><span class="sxs-lookup"><span data-stu-id="540de-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="540de-116">L’attribut correspondant (généralement employeeId) ne se réssolvant pas en un utilisateur unique dans Active Directory local ou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="540de-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="540de-117">Par exemple, deux utilisateurs ont le même employeeId dans AD et le service renvoie un code d’erreur qui indique des entrées cibles en double pour la même entrée source.</span><span class="sxs-lookup"><span data-stu-id="540de-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="540de-118">Pour consulter les journaux d’un utilisateur et d’un groupe, consultez les journaux d’approvisionnement pour un [problème avec un utilisateur spécifique.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="540de-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
