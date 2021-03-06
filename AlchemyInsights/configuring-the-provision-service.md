---
title: Configuration du service d’approvisionnement
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480748"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="9ff25-102">Configuration du service d’approvisionnement</span><span class="sxs-lookup"><span data-stu-id="9ff25-102">Configuring the Provision service</span></span>

<span data-ttu-id="9ff25-103">Pour que l’approvisionnement automatisé des utilisateurs fonctionne, Azure AD requiert des informations d’identification valides qui lui permettent de se connecter à l’API workday Web Services.</span><span class="sxs-lookup"><span data-stu-id="9ff25-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="9ff25-104">En outre, le bouton Tester la connexion de l’application Workday to AD User Provisioning valide également s’il est en mesure de se connecter à l’agent d’approvisionnement Azure AD Connect associé au domaine AD.</span><span class="sxs-lookup"><span data-stu-id="9ff25-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="9ff25-105">Si le portail Azure retourne une erreur lors de l’enregistrement des informations d’identification, suivez les étapes recommandées ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="9ff25-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="9ff25-106">Confirmez que vous avez configuré le compte d’utilisateur du système d’intégration Workday comme indiqué dans la section didacticiel Configurer l’utilisateur du système [d’intégration dans Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="9ff25-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="9ff25-107">Confirmez que le service d’agent d’approvisionnement Azure AD Connect est opérationnel sur votre serveur Windows local à l’aide de la console de gestion des services.</span><span class="sxs-lookup"><span data-stu-id="9ff25-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="9ff25-108">Vous pouvez également vérifier l’état de l’agent dans le portail Azure en cliquant sur le bouton Afficher les agents locaux.</span><span class="sxs-lookup"><span data-stu-id="9ff25-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="9ff25-109">Assurez-vous d’entrer la valeur du champ « Nom d’utilisateur de la journée de travail » au format username@workday-tenant-name.</span><span class="sxs-lookup"><span data-stu-id="9ff25-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="9ff25-110">Si le nom du client-jour est manquant, l’authentification workday échoue.</span><span class="sxs-lookup"><span data-stu-id="9ff25-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="9ff25-111">Si vous configurez l’intégration avec le client d’implémentation Workday, notez les heures d’arrêt prévues de votre client Workday.</span><span class="sxs-lookup"><span data-stu-id="9ff25-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="9ff25-112">Workday a programmé des temps d’arrêt pour ses locataires d’implémentation pendant les week-ends (généralement du vendredi soir au samedi matin) et les échecs de connectivité pendant cette fenêtre de temps d’arrêt sont un problème connu qui se résout automatiquement dès que les locataires d’implémentation sont de nouveau en ligne.</span><span class="sxs-lookup"><span data-stu-id="9ff25-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="9ff25-113">Dans de rares cas, vous pouvez également voir cette erreur si le mot de passe de l’utilisateur du système d’intégration a changé en raison de l’actualisation du client ou si le compte est dans un état verrouillé ou expiré.</span><span class="sxs-lookup"><span data-stu-id="9ff25-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="9ff25-114">Vérifiez l’état de l’utilisateur du système d’intégration auprès de votre administrateur workday.</span><span class="sxs-lookup"><span data-stu-id="9ff25-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="9ff25-115">Pour plus d’informations sur la configuration de la journée de travail pour l’approvisionnement automatisé, voir Didacticiel : Configurer Workday pour la mise en service [automatique des utilisateurs.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="9ff25-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
