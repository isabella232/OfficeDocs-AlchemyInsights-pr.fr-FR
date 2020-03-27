---
title: La règle DLP pour le numéro de compte bancaire américain ne fonctionne pas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977160"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="5d6e4-102">Problèmes liés à DLP avec les numéros de compte bancaire américain</span><span class="sxs-lookup"><span data-stu-id="5d6e4-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="5d6e4-103">**Important**: pendant ces temps inégalés, nous faisons en sorte de s’assurer que les services SharePoint Online et OneDrive restent hautement disponibles : consultez les [ajustements de fonctionnalité temporaire SharePoint Online](https://aka.ms/ODSPAdjustments) pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="5d6e4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5d6e4-104">**Problèmes liés à DLP avec les numéros de compte bancaire américain**</span><span class="sxs-lookup"><span data-stu-id="5d6e4-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="5d6e4-105">Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de compte bancaire américain** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ?</span><span class="sxs-lookup"><span data-stu-id="5d6e4-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5d6e4-106">Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lors de l’évaluation.</span><span class="sxs-lookup"><span data-stu-id="5d6e4-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="5d6e4-107">Par exemple, pour une stratégie de **numéro de compte bancaire américain** configurée avec un niveau de confiance de 85%, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche :</span><span class="sxs-lookup"><span data-stu-id="5d6e4-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="5d6e4-108">**[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 chiffres</span><span class="sxs-lookup"><span data-stu-id="5d6e4-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="5d6e4-109">**[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 chiffres consécutifs.</span><span class="sxs-lookup"><span data-stu-id="5d6e4-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="5d6e4-110">**[Checksum :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’y a pas de checksum</span><span class="sxs-lookup"><span data-stu-id="5d6e4-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="5d6e4-111">**[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Une stratégie DLP est sûre à 75% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :</span><span class="sxs-lookup"><span data-stu-id="5d6e4-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5d6e4-112">L’expression régulière Regex_usa_bank_account_number trouve le contenu qui correspond au modèle</span><span class="sxs-lookup"><span data-stu-id="5d6e4-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="5d6e4-113">Un mot clé figurant dans la liste Keyword_usa_Bank_Account est trouvé.</span><span class="sxs-lookup"><span data-stu-id="5d6e4-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="5d6e4-114">Par exemple, l’exemple suivant se déclenche pour la stratégie de **numéro de compte bancaire américain** : compte courant 78344011</span><span class="sxs-lookup"><span data-stu-id="5d6e4-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="5d6e4-115">Pour plus d’informations sur les éléments requis pour la détection d’un **numéro de compte bancaire américain** pour votre contenu, reportez-vous à la section suivante de cet article : [ce que recherche les types d’informations sensibles pour le numéro de compte bancaire américain](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="5d6e4-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="5d6e4-116">À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5d6e4-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  