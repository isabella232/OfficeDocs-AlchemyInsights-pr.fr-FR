---
title: Ajouter des utilisateurs externes à un groupe de distribution?
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce67797a1838630ab3a42e1eeeefc401a0e3f753
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398456"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="fdcdb-102">Ajouter des utilisateurs externes à un groupe de distribution?</span><span class="sxs-lookup"><span data-stu-id="fdcdb-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="fdcdb-103">L'ajout d'un contact externe à un groupe de distribution (DG) est un processus en deux étapes:</span><span class="sxs-lookup"><span data-stu-id="fdcdb-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="fdcdb-104">Créez un contact de messagerie pour l'utilisateur externe:</span><span class="sxs-lookup"><span data-stu-id="fdcdb-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="fdcdb-105">Cliquez [ici](https://admin.microsoft.com/adminportal/home#/Contact) pour accéder à la page modifier le contact dans le portail d'administration.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="fdcdb-106">Cliquez sur **Ajouter un contact**.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="fdcdb-107">Tapez les informations pour votre contact, puis cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="fdcdb-108">Ajoutez le contact de messagerie à votre DG:</span><span class="sxs-lookup"><span data-stu-id="fdcdb-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="fdcdb-109">Cliquez [ici](https://admin.microsoft.com/adminportal/home#/groups) pour accéder à la page groupes.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="fdcdb-110">Recherchez le DG auquel vous souhaitez ajouter l'utilisateur externe, puis cliquez dessus pour ouvrir la boîte de dialogue Modifier.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="fdcdb-111">Cliquez sur le bouton **modifier** dans la liste **membres** .</span><span class="sxs-lookup"><span data-stu-id="fdcdb-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="fdcdb-112">Cliquez sur **Ajouter des membres**.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="fdcdb-113">Sélectionnez le contact de messagerie que vous avez créé à l'étape précédente, puis cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="fdcdb-114">Si même après avoir suivi ces étapes, vos utilisateurs externes ne peuvent pas envoyer de courriers électroniques au DG ou ne reçoivent pas de courriers électroniques, c'est que le DG est marqué pour autoriser uniquement les messages provenant d'utilisateurs internes.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="fdcdb-115">Vous pouvez vérifier cette configuration et la corriger en suivant les instructions [ici](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fdcdb-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="fdcdb-116">**Remarque:** Ces instructions ne s'appliquent pas si le type de votre groupe est «groupe Office 365» au lieu de «groupe de distribution».</span><span class="sxs-lookup"><span data-stu-id="fdcdb-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="fdcdb-117">Si c'est le cas, vous pouvez ajouter l'utilisateur externe directement au groupe à partir d'Outlook ou d'Outlook sur le Web.</span><span class="sxs-lookup"><span data-stu-id="fdcdb-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="fdcdb-118">Vous trouverez des explications détaillées sur les groupes Office 365 invités ainsi que des instructions pour l'ajout d'invités externes dans [cet article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="fdcdb-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  

