---
title: Problème de jointage de MVs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884587"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="51e22-102">Problème de jointage de MVs</span><span class="sxs-lookup"><span data-stu-id="51e22-102">Issue joining VMs</span></span>

<span data-ttu-id="51e22-103">Pour résoudre les problèmes qui se produisent lorsque vous tentez de joindre des MV, effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="51e22-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="51e22-104">Essayez de vous connectez à l’aide du format **UPN** (par exemple, « joeuser@contoso.com »). Au lieu du format **SAMAccountName** ('CONTOSO\joeuser').</span><span class="sxs-lookup"><span data-stu-id="51e22-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="51e22-105">Assurez-vous d’activer la synchronisation des mots de passe conformément aux étapes décrites dans le guide de *Mise en route* .</span><span class="sxs-lookup"><span data-stu-id="51e22-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="51e22-106">Assurez-vous que le compte d’utilisateur affecté n’est pas un compte externe dans le client Azure AD.</span><span class="sxs-lookup"><span data-stu-id="51e22-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="51e22-107">Les utilisateurs externes ne peuvent pas se connecter au domaine géré, car Azure AD Domain Services ne comprend pas d’informations d’identification pour ces comptes d’utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="51e22-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="51e22-108">Si le compte d’utilisateur concerné est un compte d’utilisateur réservé au cloud, assurez-vous que les utilisateurs ont modifié leur mot de passe après avoir activé les services de domaine Azure AD.</span><span class="sxs-lookup"><span data-stu-id="51e22-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="51e22-109">Les informations d’identification requises pour les services de domaine Azure AD sont alors générées à l’aide de cette étape.</span><span class="sxs-lookup"><span data-stu-id="51e22-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="51e22-110">Si les comptes d’utilisateurs affectés sont synchronisés à partir d’un annuaire local, vérifiez que la publication recommandée d’Azure AD Connect a été configurée pour effectuer une synchronisation complète.</span><span class="sxs-lookup"><span data-stu-id="51e22-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="51e22-111">Si les problèmes persistent après la confirmation de l’étape 4, exécutez les commandes suivantes à partir de votre ordinateur de synchronisation :</span><span class="sxs-lookup"><span data-stu-id="51e22-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="51e22-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="51e22-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>