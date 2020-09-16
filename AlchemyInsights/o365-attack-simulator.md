---
title: 2681 simulateur d’attaque dans Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759217"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="e3681-102">Simulateur d’attaque dans Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e3681-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="e3681-103">Vous ne disposez pas d’un simulateur d’attaque ?</span><span class="sxs-lookup"><span data-stu-id="e3681-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="e3681-104">Le simulateur d’attaque nécessite **office 365 Advanced Threat Protection Plan 2 (ATP plan 2)** ou **Office 365 entreprise E5**.</span><span class="sxs-lookup"><span data-stu-id="e3681-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="e3681-105">Le simulateur d’attaque n’est **pas** inclus dans Office 365 Advanced Threat Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3 ou tout abonnement aux applications Microsoft 365 apps pour les entreprises.</span><span class="sxs-lookup"><span data-stu-id="e3681-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="e3681-106">Le compte que vous utilisez pour lancer des attaques simulées requiert des autorisations d’administrateur général ou d’administrateur de sécurité, ainsi qu’une authentification multifacteur (MFA).</span><span class="sxs-lookup"><span data-stu-id="e3681-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="e3681-107">Pour plus d’informations sur les exigences en matière de simulateur d’attaque, consultez [cette rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="e3681-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="e3681-108">Éléments importants à connaître sur les simulations d’attaques **de mot de passe** en force :</span><span class="sxs-lookup"><span data-stu-id="e3681-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="e3681-109">Si l’authentification multifacteur est activée pour le compte cible et que le mot de passe a été deviné correctement, le compte ne s’affichera pas comme compromis (le deuxième facteur d’authentification sera incomplet).</span><span class="sxs-lookup"><span data-stu-id="e3681-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="e3681-110">Le fichier de mot de passe ne peut pas être supérieur à 10 Mo.</span><span class="sxs-lookup"><span data-stu-id="e3681-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="e3681-111">Utilisez un mot de passe par ligne et incluez une ligne vide (retour chariot) après le dernier mot de passe de la liste.</span><span class="sxs-lookup"><span data-stu-id="e3681-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="e3681-112">Éléments importants à connaître sur les simulations d’attachement de **Spear Phishing** :</span><span class="sxs-lookup"><span data-stu-id="e3681-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="e3681-113">Par défaut, vous ne pouvez pas fournir de valeur personnalisée pour l' **URL du serveur de connexion d’hameçonnage**.</span><span class="sxs-lookup"><span data-stu-id="e3681-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="e3681-114">Si un destinataire utilise le [complément activer le message de rapport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pour signaler le message comme hameçonnage, il se peut que vous ne receviez pas d’alertes pour le message (car il s’agit d’une attaque simulée).</span><span class="sxs-lookup"><span data-stu-id="e3681-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="e3681-115">Rapports : une fois l’attaque simulée terminée, vous pouvez cliquer sur détails de l' **attaque** pour afficher le rapport.</span><span class="sxs-lookup"><span data-stu-id="e3681-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="e3681-116">Pour obtenir des instructions détaillées et de nouvelles fonctionnalités dans le simulateur d’attaque, consultez la rubrique [attaques de simulateur dans Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="e3681-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
