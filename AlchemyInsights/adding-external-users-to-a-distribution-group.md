---
title: Ajout d’utilisateurs externes à un groupe de distribution
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660790"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="d70e3-102">Ajouter des utilisateurs externes à un groupe de distribution</span><span class="sxs-lookup"><span data-stu-id="d70e3-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="d70e3-103">L’ajout d’un contact externe à un groupe de distribution (DG) est un processus en deux étapes:</span><span class="sxs-lookup"><span data-stu-id="d70e3-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="d70e3-104">Créez un contact de messagerie pour l’utilisateur externe:</span><span class="sxs-lookup"><span data-stu-id="d70e3-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="d70e3-105">Dans le centre d’administration, accédez à la page des[contacts](https://admin.microsoft.com/adminportal/home#/Contact) de l' **utilisateur** > .</span><span class="sxs-lookup"><span data-stu-id="d70e3-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="d70e3-106">Sélectionnez **Ajouter un contact**.</span><span class="sxs-lookup"><span data-stu-id="d70e3-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="d70e3-107">Tapez les informations relatives à votre contact, puis sélectionnez **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="d70e3-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="d70e3-108">Ajoutez le contact de messagerie à votre DG:</span><span class="sxs-lookup"><span data-stu-id="d70e3-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="d70e3-109">Dans le centre d’administration, accédez à \*\*\*\* > [](https://admin.microsoft.com/adminportal/home#/groups) la page groupes de groupes.</span><span class="sxs-lookup"><span data-stu-id="d70e3-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="d70e3-110">Recherchez le DG auquel vous souhaitez ajouter l’utilisateur externe, puis sélectionnez-le pour ouvrir la boîte de dialogue Modifier.</span><span class="sxs-lookup"><span data-stu-id="d70e3-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="d70e3-111">Sous l’onglet **membres** , sélectionnez **Afficher tout et gérer les membres**.</span><span class="sxs-lookup"><span data-stu-id="d70e3-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="d70e3-112">Sélectionnez **Ajouter des membres**.</span><span class="sxs-lookup"><span data-stu-id="d70e3-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="d70e3-113">Sélectionnez le contact de messagerie que vous avez créé à l’étape précédente, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="d70e3-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="d70e3-114">Si, après avoir suivi ces étapes, vos utilisateurs externes ne peuvent pas envoyer de courriers électroniques au DG ou ne reçoivent pas de courriers électroniques, il est possible que le DG soit marqué pour autoriser uniquement les messages provenant d’utilisateurs internes.</span><span class="sxs-lookup"><span data-stu-id="d70e3-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="d70e3-115">Vous pouvez vérifier cette configuration et la corriger en suivant les instructions fournies [ici](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="d70e3-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="d70e3-116">**Remarque:** Ces instructions ne s’appliquent pas si le type de votre groupe est «groupe Office 365» au lieu de «groupe de distribution».</span><span class="sxs-lookup"><span data-stu-id="d70e3-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="d70e3-117">Dans ce cas, vous pouvez ajouter l’utilisateur externe directement au groupe à partir d’Outlook.</span><span class="sxs-lookup"><span data-stu-id="d70e3-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="d70e3-118">Vous trouverez des informations détaillées sur les groupes Office 365 invités ainsi que des instructions pour l’ajout d’invités externes dans [cet article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="d70e3-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  