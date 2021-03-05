---
title: Synchronisation des mots de passe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449085"
---
# <a name="password-synchronization"></a><span data-ttu-id="642ad-102">Synchronisation des mots de passe</span><span class="sxs-lookup"><span data-stu-id="642ad-102">Password synchronization</span></span>

<span data-ttu-id="642ad-103">**La synchronisation de hachage de mot de passe ne fonctionne pas du tout**</span><span class="sxs-lookup"><span data-stu-id="642ad-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="642ad-104">Voici quelques problèmes courants rencontrés par les clients lorsque la synchronisation de hachage de mot de passe ne fonctionne pas :</span><span class="sxs-lookup"><span data-stu-id="642ad-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="642ad-105">Le compte Active Directory utilisé par Azure AD Connect pour communiquer avec  Active Directory  local n’est pas autorisé à répliquer les modifications d’annuaire et répliquer les changements de répertoire Toutes les autorisations requises pour la synchronisation de mot de passe. Vous devez résoudre ce problème en accordant ces autorisations au compte Active Directory.</span><span class="sxs-lookup"><span data-stu-id="642ad-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="642ad-106">La synchronisation de hachage de mot de passe est  désactivée après qu’un administrateur a modifié la méthode User Sign-In de synchronisation de mot  de passe à une autre option telle que la fédération avec **AD FS** dans l’Assistant Azure AD Connect . Vous pouvez résoudre ce problème en réactivant la fonctionnalité de synchronisation de hachage de mot de passe dans l’Assistant Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="642ad-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="642ad-107">Problème de connectivité avec Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="642ad-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="642ad-108">Par exemple, certains contrôleurs de domaine ne sont pas accessibles par Azure AD Connect ou les [ports](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) requis sont bloqués par le pare-feu. Vous devez résoudre ce problème en vous assurant que la connectivité entre le serveur Azure AD Connect et l’active Directory local fonctionne correctement.</span><span class="sxs-lookup"><span data-stu-id="642ad-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="642ad-109">Le serveur Azure AD Connect est actuellement en mode intermédiaire, ce qui permettra au serveur de ne pas être en mesure d’utiliser les hésages de mot de passe . Pour résoudre le problème, suivez les étapes décrites dans la section Résoudre les problèmes de synchronisation de mot de passe avec la synchronisation [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)- Aucun mot de passe n’est synchronisé.</span><span class="sxs-lookup"><span data-stu-id="642ad-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="642ad-110">**La synchronisation de hachage de mot de passe ne fonctionne pas pour certains de mes utilisateurs**</span><span class="sxs-lookup"><span data-stu-id="642ad-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="642ad-111">Si vous avez remarqué que le hachage de  mot de passe n’est pas synchronisé pour un utilisateur, utilisez la tâche de dépannage dans Azure AD Connect pour examiner et résoudre le problème.</span><span class="sxs-lookup"><span data-stu-id="642ad-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="642ad-112">Effectuez les tâches suivantes :</span><span class="sxs-lookup"><span data-stu-id="642ad-112">Perform the following tasks:</span></span>

    <span data-ttu-id="642ad-113">a.</span><span class="sxs-lookup"><span data-stu-id="642ad-113">a.</span></span> [<span data-ttu-id="642ad-114">Exécuter la tâche de dépannage dans l’Assistant</span><span class="sxs-lookup"><span data-stu-id="642ad-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="642ad-115">b.</span><span class="sxs-lookup"><span data-stu-id="642ad-115">b.</span></span> [<span data-ttu-id="642ad-116">Utiliser la cmdlet de dépannage pour examiner le problème de synchronisation de hachage de mot de passe pour une utilisation spécifique</span><span class="sxs-lookup"><span data-stu-id="642ad-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="642ad-117">L’objet utilisateur Active Directory local est activé pour l’utilisateur doit modifier le mot de passe à la prochaine option **d’accès.**</span><span class="sxs-lookup"><span data-stu-id="642ad-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="642ad-118">Lorsque cette option est activée, un mot de passe temporaire est attribué à l’utilisateur et est invité à le modifier lors de la prochaine fermeture de site.</span><span class="sxs-lookup"><span data-stu-id="642ad-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="642ad-119">Azure AD Connect ne synchronise pas les mots de passe temporaires avec Azure AD.</span><span class="sxs-lookup"><span data-stu-id="642ad-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="642ad-120">Pour résoudre le problème ci-dessus, effectuez l’une des tâches suivantes :</span><span class="sxs-lookup"><span data-stu-id="642ad-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="642ad-121">Demandez à l’utilisateur de se connectez à l’application sur site (par exemple, Windows Desktop) et modifiez le mot de passe.</span><span class="sxs-lookup"><span data-stu-id="642ad-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="642ad-122">Le nouveau mot de passe sera synchronisé avec Azure AD.</span><span class="sxs-lookup"><span data-stu-id="642ad-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="642ad-123">Permettre à un administrateur de mettre à jour le mot de passe de l’utilisateur sans activer l’option L’utilisateur doit modifier le mot de passe à la prochaine **logonisation** et partager le nouveau mot de passe avec l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="642ad-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="642ad-124">L’objet Utilisateur Active Directory  local n’est pas correctement configuré pour la synchronisation d’objets ou la synchronisation de mot de passe.</span><span class="sxs-lookup"><span data-stu-id="642ad-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="642ad-125">Pour résoudre ce problème, suivez les étapes décrites dans la résolution des problèmes de synchronisation de hachage de mot de passe avec la synchronisation [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="642ad-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







