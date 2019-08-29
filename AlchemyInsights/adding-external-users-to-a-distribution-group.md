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
# <a name="add-external-users-to-a-distribution-group"></a>Ajouter des utilisateurs externes à un groupe de distribution

L’ajout d’un contact externe à un groupe de distribution (DG) est un processus en deux étapes:
  
1. Créez un contact de messagerie pour l’utilisateur externe:
    
    1. Dans le centre d’administration, accédez à la page des[contacts](https://admin.microsoft.com/adminportal/home#/Contact) de l' **utilisateur** > . 
    
    2. Sélectionnez **Ajouter un contact**.
    
    3. Tapez les informations relatives à votre contact, puis sélectionnez **Ajouter**.
    
2. Ajoutez le contact de messagerie à votre DG:
    
    1. Dans le centre d’administration, accédez à **** > [](https://admin.microsoft.com/adminportal/home#/groups) la page groupes de groupes. 
    
    2. Recherchez le DG auquel vous souhaitez ajouter l’utilisateur externe, puis sélectionnez-le pour ouvrir la boîte de dialogue Modifier.
    
    3. Sous l’onglet **membres** , sélectionnez **Afficher tout et gérer les membres**. 
    
    4. Sélectionnez **Ajouter des membres**.
    
    5. Sélectionnez le contact de messagerie que vous avez créé à l’étape précédente, puis sélectionnez **Enregistrer**.
    
Si, après avoir suivi ces étapes, vos utilisateurs externes ne peuvent pas envoyer de courriers électroniques au DG ou ne reçoivent pas de courriers électroniques, il est possible que le DG soit marqué pour autoriser uniquement les messages provenant d’utilisateurs internes. Vous pouvez vérifier cette configuration et la corriger en suivant les instructions fournies [ici](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Remarque:** Ces instructions ne s’appliquent pas si le type de votre groupe est «groupe Office 365» au lieu de «groupe de distribution». Dans ce cas, vous pouvez ajouter l’utilisateur externe directement au groupe à partir d’Outlook. Vous trouverez des informations détaillées sur les groupes Office 365 invités ainsi que des instructions pour l’ajout d’invités externes dans [cet article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  