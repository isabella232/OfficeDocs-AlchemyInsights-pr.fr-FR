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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680133"
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