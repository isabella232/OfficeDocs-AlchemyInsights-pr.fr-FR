---
title: Ajout d’utilisateurs externes à un groupe de distribution
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934831"
---
# <a name="add-external-users-to-a-distribution-group"></a>Ajouter des utilisateurs externes à un groupe de distribution

L’ajout d’un contact externe à un groupe de distribution est un processus en deux étapes :
  
1. Créez un contact de messagerie pour l’utilisateur externe :
    
    1. Dans le centre d’administration, allez à **la**  >  page Contacts des [utilisateurs.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Sélectionnez **Ajouter un contact.**
    
    3. Tapez les informations de votre contact, puis sélectionnez **Ajouter.**
    
2. Ajoutez le contact de messagerie à votre DG :
    
    1. Dans le Centre d’administration, allez à la page   >  [Groupes.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Recherchez le DG à ajouter à l’utilisateur externe, puis sélectionnez-le pour ouvrir la boîte de dialogue d’édition.
    
    3. Sous **l’onglet Membres,** **sélectionnez Afficher tout et gérer les membres.** 
    
    4. Sélectionnez **Ajouter des membres**.
    
    5. Sélectionnez le contact de messagerie que vous avez créé à l’étape précédente, puis sélectionnez **Enregistrer.**
    
Si, après avoir suivi ces étapes, vos utilisateurs externes ne peuvent pas envoyer de courriers électroniques au groupe de sécurité ou ne reçoivent pas de courriers électroniques de celui-ci, il se peut que le DG soit marqué pour autoriser uniquement les e-mails provenant d’utilisateurs internes. Vous pouvez vérifier cette configuration et la corriger en suivant les instructions [ci-après.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Remarque :** Ces instructions ne s’appliquent pas si le type de votre groupe est « Microsoft 365 groupe » au lieu de « Groupe de distribution ». Si c’est le cas, vous pouvez ajouter l’utilisateur externe directement au groupe à partir de Outlook. Des informations détaillées sur Microsoft 365 groupes invités, ainsi que des instructions pour l’ajout d’invités externes sont disponibles [dans cet article.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  