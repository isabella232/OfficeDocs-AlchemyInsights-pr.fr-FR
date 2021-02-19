---
title: Vos utilisateurs ont reçu des messages malveillants ?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291790"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="6cf43-102">Vos utilisateurs ont reçu des messages malveillants ?</span><span class="sxs-lookup"><span data-stu-id="6cf43-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="6cf43-103">Vous pouvez désormais signaler l’e-mail malveillant à Microsoft à l’aide des [soumissions d’administrateur dans le Centre de sécurité et de conformité](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="6cf43-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="6cf43-104">Le programme analyse les messages envoyés dans des soumissions [d'administrateur](https://sip.protection.office.com/reportsubmission), et les résultats suivants apparaissent dans le menu volant **Détails** :</span><span class="sxs-lookup"><span data-stu-id="6cf43-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="6cf43-105">En cas d’échec de l’authentification des e-mails de l’expéditeur au moment de la livraison.</span><span class="sxs-lookup"><span data-stu-id="6cf43-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="6cf43-106">Informations sur les accès à la stratégie qui auraient pu affecter ou écraser le verdict d’un message.</span><span class="sxs-lookup"><span data-stu-id="6cf43-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="6cf43-107">Résultats actuels de la détonation pour savoir si les URL ou fichiers contenus dans le message étaient malveillants ou non.</span><span class="sxs-lookup"><span data-stu-id="6cf43-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="6cf43-108">Commentaires des grilles d’évaluation</span><span class="sxs-lookup"><span data-stu-id="6cf43-108">Feedback from graders</span></span>

<span data-ttu-id="6cf43-109">Si le programme a trouvé un remplacement, la nouvelle analyse doit se terminer après plusieurs minutes.</span><span class="sxs-lookup"><span data-stu-id="6cf43-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="6cf43-110">Si le programme n’a pas rencontré de problème dans l’authentification d’e-mails ou si aucun remplacement n’a affecté la livraison, les commentaires des évaluateurs peuvent prendre jusqu’à un jour.</span><span class="sxs-lookup"><span data-stu-id="6cf43-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="6cf43-111">Si vous n’êtes pas d’accord avec le verdict sur un message, une URL ou un fichier (bloqué ou non), envoyez de nouveau le message après un jour pour nouvelle analyse.</span><span class="sxs-lookup"><span data-stu-id="6cf43-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="6cf43-112">Le verdict a toutes les chances de changer après le nouvel envoi du message.</span><span class="sxs-lookup"><span data-stu-id="6cf43-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="6cf43-113">Pendant ce temps, vous pouvez supprimez les e-mails malveillants des boîtes de réception des utilisateurs en suivant les instructions de [cet article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="6cf43-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="6cf43-114">Les clients qui disposent de Microsoft Defender pour Office 365 peuvent :</span><span class="sxs-lookup"><span data-stu-id="6cf43-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="6cf43-115">Utiliser l’[Explorateur de menaces pour rechercher, puis supprimer les e-mails suspects](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="6cf43-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="6cf43-116">[utiliser la fonction Liens fiables pour bloquer l'accès](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) à une URL malveillante</span><span class="sxs-lookup"><span data-stu-id="6cf43-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="6cf43-117">suivre les utilisateurs qui ont cliqué sur des URL malveillantes, puis y ont accédé : [Afficher l’URL de phishing et cliquer sur les données du verdict](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="6cf43-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="6cf43-118">démarrer manuellement [une analyse automatisée](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="6cf43-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="6cf43-119">Vous pouvez également vous protéger contre les fichiers et les URL malveillants en suivant les instructions fournies dans [Protection contre les URL et fichiers malveillants](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="6cf43-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>