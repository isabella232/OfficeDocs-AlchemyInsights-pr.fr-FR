---
title: Simulateur d’attaques 2681 dans Microsoft 365
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545724"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="bac65-102">Simulateur d’attaques dans Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bac65-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="bac65-103">Le Simulateur d’attaques vous manque ?</span><span class="sxs-lookup"><span data-stu-id="bac65-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="bac65-104">Le Simulateur d’attaques **nécessite Microsoft Defender Office 365 plan 2** ou Office 365 Entreprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="bac65-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="bac65-105">Le Simulateur  d’attaques n’est pas inclus dans Microsoft Defender pour Office 365 Plan 1, Office 365 Entreprise E3 ou les abonnements Applications Microsoft 365 pour les PME de service.</span><span class="sxs-lookup"><span data-stu-id="bac65-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="bac65-106">Le compte que vous utilisez pour lancer des attaques simulées nécessite des autorisations d’administrateur général ou d’administrateur de sécurité et une authentification multifacteur (MFA).</span><span class="sxs-lookup"><span data-stu-id="bac65-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="bac65-107">Pour plus d’informations sur les exigences du simulateur d’attaques, [consultez cette rubrique.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="bac65-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="bac65-108">Points importants à connaître sur les simulations d’attaques **par mot** de passe en force brute :</span><span class="sxs-lookup"><span data-stu-id="bac65-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="bac65-109">Si l’authentification multifacteur est activée sur le compte cible et que le mot de passe a été deviné correctement, le compte ne sera pas compromis (le deuxième facteur d’authentification sera incomplet).</span><span class="sxs-lookup"><span data-stu-id="bac65-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="bac65-110">Le fichier de mot de passe ne peut pas être supérieur à 10 Mo.</span><span class="sxs-lookup"><span data-stu-id="bac65-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="bac65-111">Utilisez un mot de passe par ligne et incluez une ligne vide (retour chariot) après le dernier mot de passe de la liste.</span><span class="sxs-lookup"><span data-stu-id="bac65-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="bac65-112">Points importants à connaître sur les simulations d’attachement de **harponnage** :</span><span class="sxs-lookup"><span data-stu-id="bac65-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="bac65-113">Par conception, vous ne pouvez pas fournir de valeur personnalisée pour l’URL du serveur de connexion au **hameçonnage.**</span><span class="sxs-lookup"><span data-stu-id="bac65-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="bac65-114">Si un destinataire utilise le [add-in Activer](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) le message de rapport pour signaler le message comme hameçonnage, il se peut que vous ne receviez pas d’alertes pour le message (car il s’agit d’une attaque simulée).</span><span class="sxs-lookup"><span data-stu-id="bac65-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="bac65-115">Rapports : une fois l’attaque simulée terminée, vous pouvez cliquer sur **Détails** de l’attaque pour voir le rapport.</span><span class="sxs-lookup"><span data-stu-id="bac65-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="bac65-116">Pour obtenir des instructions détaillées et de nouvelles fonctionnalités dans le Simulateur d’attaques, voir Simulateur [d’attaques dans Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="bac65-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
