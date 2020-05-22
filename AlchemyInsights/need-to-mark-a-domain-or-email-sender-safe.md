---
title: Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281146"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="49975-102">Vous devez marquer un domaine ou un expéditeur de courrier comme sécurisé ?</span><span class="sxs-lookup"><span data-stu-id="49975-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="49975-103">L’utilisation de **listes d’expéditeurs approuvés n’est pas recommandé** car elle ouvre votre organisation aux attaques d’usurpation d’identité, de hameçonnage et au courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="49975-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="49975-104">Toutefois, s’il existe un besoin d’entreprise, nous vous **recommandons** l’utilisation de **[Règles de flux de courrier](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**.</span><span class="sxs-lookup"><span data-stu-id="49975-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="49975-105">Nos recommandations garantissent l’authentification de l’expéditeur (vérification que le domaine expéditeur n’est pas usurpé).</span><span class="sxs-lookup"><span data-stu-id="49975-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="49975-106">**Remarque** : nous vous déconseillons de gérer les faux positifs à l’aide de listes d’expéditeurs approuvés, car les exceptions au filtrage du courrier indésirable peuvent ouvrir votre organisation à des attaques au niveau de la sécurité.</span><span class="sxs-lookup"><span data-stu-id="49975-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="49975-107">Si vos utilisateurs reçoivent des messages incorrectement marqués comme courrier indésirable, veuillez **[Signaler les messages et fichiers à Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="49975-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="49975-108">Les expéditeurs approuvés dans Outlook, la liste des expéditeurs autorisés ou la liste de domaines autorisés dans les stratégies anti-courrier indésirable **doivent être évités** car les expéditeurs ignorent la protection contre le courrier indésirable, l’usurpation d’identité et l’authentification de l’expéditeur (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="49975-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="49975-109">Cette méthode est idéale pour les tests temporaires uniquement.</span><span class="sxs-lookup"><span data-stu-id="49975-109">This method is best used for temporary testing only.</span></span>
