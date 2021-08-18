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
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088070"
---
# <a name="issue-joining-vms"></a>Problème de jointage de MVs

Pour résoudre les problèmes qui se produisent lorsque vous tentez de joindre des MV, effectuez les étapes suivantes :

1. Essayez de vous connectez à l’aide du format **UPN** (par exemple, « joeuser@contoso.com »). Au lieu du format **SAMAccountName** ('CONTOSO\joeuser').
2. Assurez-vous d’activer la synchronisation des mots de passe conformément aux étapes décrites dans le guide de *Mise en route* .
3. Assurez-vous que le compte d’utilisateur affecté n’est pas un compte externe dans le client Azure AD. Les utilisateurs externes ne peuvent pas se connecter au domaine géré, car Azure AD Domain Services ne comprend pas d’informations d’identification pour ces comptes d’utilisateurs.
4. Si le compte d’utilisateur concerné est un compte d’utilisateur réservé au cloud, assurez-vous que les utilisateurs ont modifié leur mot de passe après avoir activé les services de domaine Azure AD. Les informations d’identification requises pour les services de domaine Azure AD sont alors générées à l’aide de cette étape.
5. Si les comptes d’utilisateurs affectés sont synchronisés à partir d’un annuaire local, vérifiez que la publication recommandée d’Azure AD Connect a été configurée pour effectuer une synchronisation complète.
6. Si les problèmes persistent après la confirmation de l’étape 4, exécutez les commandes suivantes à partir de votre ordinateur de synchronisation :
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.