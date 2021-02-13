---
title: L’écriture écriture par mot de passe ne fonctionne pas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232719"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="d21b3-102">L’écriture écriture par mot de passe ne fonctionne pas</span><span class="sxs-lookup"><span data-stu-id="d21b3-102">Password Writeback is not working</span></span>

<span data-ttu-id="d21b3-103">**J’ai des difficultés à configurer l’écriture écriture par mot de passe**</span><span class="sxs-lookup"><span data-stu-id="d21b3-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="d21b3-104">L’écriture écriture par mot de passe est une fonctionnalité importante.</span><span class="sxs-lookup"><span data-stu-id="d21b3-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="d21b3-105">Assurez-vous de bien comprendre les exigences de licence :</span><span class="sxs-lookup"><span data-stu-id="d21b3-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="d21b3-106">Vous devez avoir au moins une licence attribuée dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="d21b3-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="d21b3-107">**Utilisateurs cloud uniquement** : toute référence (SKU) payante Office 365 (O365) ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="d21b3-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="d21b3-108">**Utilisateurs cloud et/ou** locaux : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="d21b3-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="d21b3-109">Pour en savoir plus sur les exigences en matière de licences, consultez La gestion des licences requise pour la réinitialisation du mot de passe en [libre-service Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="d21b3-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="d21b3-110">Vous avez au moins un compte d’administrateur et un compte d’utilisateur test avec l’une des licences appropriées.</span><span class="sxs-lookup"><span data-stu-id="d21b3-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="d21b3-111">Vous devez connecter Azure AD Connect à l’émulateur du contrôleur de domaine principal pour que l’écriture écriture par mot de passe fonctionne.</span><span class="sxs-lookup"><span data-stu-id="d21b3-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="d21b3-112">Vous pouvez configurer Azure AD Connect pour utiliser un contrôleur  de domaine principal en cliquant avec le bouton droit sur les propriétés du connecteur de synchronisation Active Directory, puis en sélectionnant configurer les **partitions** d’annuaire.</span><span class="sxs-lookup"><span data-stu-id="d21b3-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="d21b3-113">À partir de là, recherchez la section **paramètres** de connexion du contrôleur de domaine et cochez la case intitulée utiliser uniquement les **contrôleurs de domaine préférés.**</span><span class="sxs-lookup"><span data-stu-id="d21b3-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="d21b3-114">Si le dc préféré n’est pas un émulateur PDC, Azure AD Connect contacte toujours le PDC pour l’écriture de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="d21b3-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="d21b3-115">La réinitialisation du mot de passe a été configurée et activée dans votre client.</span><span class="sxs-lookup"><span data-stu-id="d21b3-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="d21b3-116">Pour plus d’informations, voir [Permettre aux utilisateurs de réinitialiser leurs mots de passe Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="d21b3-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="d21b3-117">Assurez-vous que le compte d’administrateur utilisé pour activer l’écriture par mot de passe est un compte d’administrateur cloud (créé dans Azure AD et non dans AD local)</span><span class="sxs-lookup"><span data-stu-id="d21b3-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="d21b3-118">Vous avez un déploiement AD sur site à forêts multiples ou unique exécutant Windows Server 2008 R2, Windows Server 2012 ou Windows Server 2012 R2 avec les derniers Service Packs installés.</span><span class="sxs-lookup"><span data-stu-id="d21b3-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="d21b3-119">L’outil Azure AD Connect est installé et vous avez préparé votre environnement AD pour la synchronisation avec le cloud.</span><span class="sxs-lookup"><span data-stu-id="d21b3-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="d21b3-120">Avant de tester l’écriture écriture par mot de passe, assurez-vous d’abord d’effectuer une importation complète et une synchronisation complète à partir d’AD et d’Azure AD dans Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d21b3-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="d21b3-121">Pour en savoir plus, découvrez comment faire une synchronisation complète et une [importation complète dans Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="d21b3-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="d21b3-122">**J’ai un problème avec la connectivité d’écriture/écriture de mot de passe**</span><span class="sxs-lookup"><span data-stu-id="d21b3-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="d21b3-123">Télécharger et activer la dernière version [d’Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="d21b3-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="d21b3-124">Configuration du pare-feu : l’outil Azure AD Connect (1.1.443 et supérieur) aura besoin d’un accès **HTTPS** sortant pour :</span><span class="sxs-lookup"><span data-stu-id="d21b3-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="d21b3-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d21b3-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="d21b3-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="d21b3-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="d21b3-127">Autoriser la persistance des connexions inactives pendant au moins 2 à 3 minutes</span><span class="sxs-lookup"><span data-stu-id="d21b3-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="d21b3-128">**J’ai toujours des problèmes avec l’écriture écriture par mot de passe**</span><span class="sxs-lookup"><span data-stu-id="d21b3-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="d21b3-129">Si vous avez encore des difficultés, essayez de désactiver et de réactiver le service d’écriture écriture de mot de passe dans l’outil Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d21b3-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="d21b3-130">Pour plus d’informations, voir comment désactiver [et réactiver](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) l’écriture par mot de passe</span><span class="sxs-lookup"><span data-stu-id="d21b3-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
