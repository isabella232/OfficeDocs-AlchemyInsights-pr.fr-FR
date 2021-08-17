---
title: Supprimer l’utilisateur orphelin du serveur local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102247"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Supprimer l’utilisateur orphelin du serveur local

Pour supprimer un utilisateur orphelin, procédez comme suit :

1. Forcer la synchronisation d’annuaires en suivant les instructions dans [Qu’est-ce que l’identité hybride avec Azure Active Directory ?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Pour vérifier la synchronisation d’annuaires, consultez [Qu’est-ce que l’identité hybride avec Azure Active Directory ?](https://technet.microsoft.com/library/jj151797.aspx).

3. Si la synchronisation fonctionne correctement, mais que la suppression d’objets Active Directory ne se propage pas à Azure AD, supprimez manuellement l’objet orphelin à l’aide de l’un des applets de commande Module Azure Active Directory pour Windows PowerShell :

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Par exemple, pour supprimer l’ID utilisateur orphelin john.smith@contoso.com, créé à l’origine à l’aide de la synchronisation d’annuaires, exécutez l’applet de commande :

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com