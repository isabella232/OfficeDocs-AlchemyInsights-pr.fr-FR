---
title: Activer l'écriture différée de mot de passe dans Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093353"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="3e638-102">Activer l'écriture différée de mot de passe dans Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3e638-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="3e638-103">Pour activer l’écriture différée de réinitialisation de mot de passe en libre-service, commencez par activer l’option d’écriture différée dans Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3e638-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="3e638-104">À partir de votre serveur Azure AD Connect, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="3e638-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="3e638-105">Connectez-vous à votre serveur Azure AD Connect et démarrez l'assistant de configuration d’**Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="3e638-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="3e638-106">Sur la page **Bienvenue**, cliquez sur **Configurer**.</span><span class="sxs-lookup"><span data-stu-id="3e638-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="3e638-107">Sur la page **Tâches supplémentaires**, sélectionnez **Personnaliser les options de synchronisation**, puis cliquez sur **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="3e638-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="3e638-108">Sur la page Connexion à Azure AD, tapez vos informations d’identification d’administrateur général, puis cliquez sur Suivant.</span><span class="sxs-lookup"><span data-stu-id="3e638-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="3e638-109">Sur les pages **Connexion des annuaires** et **Filtrage par domaine/unité d'organisation**, cliquez sur **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="3e638-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="3e638-110">Sur la page **Fonctionnalités facultatives**, sélectionnez **Écriture différée de mot de passe** et cliquez sur **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="3e638-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="3e638-111">Sur la page **Prêt à configurer**, cliquez sur **Configurer** et attendez que le processus se termine.</span><span class="sxs-lookup"><span data-stu-id="3e638-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="3e638-112">Lorsque vous voyez que la configuration se termine, cliquez sur **Sortie**.</span><span class="sxs-lookup"><span data-stu-id="3e638-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="3e638-113">Avec l’écriture différée de mot de passe activée dans Azure AD Connect, configurez à présent Azure AD SSPR pour l’écriture différée.</span><span class="sxs-lookup"><span data-stu-id="3e638-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="3e638-114">Pour activer l’écriture différée de mot de passe dans SSPR, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="3e638-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="3e638-115">Connectez-vous au portail Azure avec votre compte Administrateur général.</span><span class="sxs-lookup"><span data-stu-id="3e638-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="3e638-116">Recherchez et sélectionnez **Azure Active Directory**, cliquez sur **Réinitialisation du mot de passe**, puis sélectionnez **Intégration locale**.</span><span class="sxs-lookup"><span data-stu-id="3e638-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="3e638-117">Définissez l’option **Réécrire des mots de passe dans votre répertoire local ?** sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="3e638-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="3e638-118">Définissez l’option **Voulez-vous autoriser les utilisateurs à déverrouiller les comptes sans réinitialiser leur mot de passe ?** sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="3e638-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="3e638-119">Lorsque vous avez fini, cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="3e638-119">When ready, click **Save**.</span></span>

<span data-ttu-id="3e638-120">Pour plus d’informations, voir [Activer l’écriture différée de réinitialisation de mot de passe en libre-service Azure Active Directory dans un environnement local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="3e638-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="3e638-121">Lorsqu’un administrateur réinitialise le mot de passe d’un utilisateur dans le portail Azure, s’il est fédéré ou si le hachage de mot de passe est synchronisé, le mot de passe est replacé dans l’instance locale.</span><span class="sxs-lookup"><span data-stu-id="3e638-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="3e638-122">Cette fonctionnalité nécessite une licence Azure Premium (P1 ou P2) et n’est actuellement pas prise en charge dans le portail d’administration Office.</span><span class="sxs-lookup"><span data-stu-id="3e638-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
