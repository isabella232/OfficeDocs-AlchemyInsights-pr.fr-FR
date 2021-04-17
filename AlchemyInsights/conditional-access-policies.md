---
title: Stratégies d’accès conditionnel
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817278"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="8aca4-102">Stratégies d’accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="8aca4-102">Conditional Access policies</span></span>

<span data-ttu-id="8aca4-103">L’accès conditionnel est une fonctionnalité d’Azure AD. Elle vous permet d’appliquer des contrôles sur l’accès aux applications dans votre environnement, le tout en fonction de conditions définies et reposant sur une gestion à partir d’un emplacement central.</span><span class="sxs-lookup"><span data-stu-id="8aca4-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="8aca4-104">En savoir plus sur l’[accès conditionnel Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="8aca4-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="8aca4-105">**Remarque** : Si votre client a été créé après le 21 octobre 2019, et si vous êtes invité à entrer une authentification multifacteur, l’option [paramètres de sécurité par défaut](https://aka.ms/securitydefaults) est certainement activée dans votre client.</span><span class="sxs-lookup"><span data-stu-id="8aca4-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="8aca4-106">**Pour gérer les paramètres de sécurité par défaut**</span><span class="sxs-lookup"><span data-stu-id="8aca4-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="8aca4-107">Connectez-vous au [centre d'administration](https://go.microsoft.com/fwlink/p/?linkid=834822) à l'aide de vos informations d'identification d'administrateur général.</span><span class="sxs-lookup"><span data-stu-id="8aca4-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="8aca4-108">Accès à [Propriétés d'Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="8aca4-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="8aca4-109">Au bas de la page, cliquez **Gérer les paramètres de sécurité par défaut**.</span><span class="sxs-lookup"><span data-stu-id="8aca4-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="8aca4-110">Cliquez sur **Oui** pour activer les paramètres de sécurité par défaut ou sur **Non** pour désactiver les paramètres de sécurité par défaut.</span><span class="sxs-lookup"><span data-stu-id="8aca4-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
