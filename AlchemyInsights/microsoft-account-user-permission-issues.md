---
title: Résoudre le problème-utilisateur introuvable dans l’annuaire
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544861"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Résoudre le problème-utilisateur introuvable dans l’annuaire

Si les utilisateurs reçoivent un message d’erreur indiquant que l’utilisateur est introuvable dans l’annuaire. Réessayez là où le type de problème est utilisateur non dans le répertoire.

Vous pouvez effectuer les étapes suivantes pour résoudre le problème.

- Assurez-vous que le compte qui a accepté l’invitation électronique est le même compte que celui utilisé pour la connexion ultérieure. Assurez-vous que l’utilisateur utilise le même compte pour accepter l’invitation et se connecter au site. 

Pour plus d’informations, reportez-vous à la rubrique [gestion</a> des alias de votre compte Microsoft pour gérer la connexion à Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Accédez à chaque site (s) dans lequel l’utilisateur reçoit l’erreur. 

Ajoutez «/_layouts/15/People.aspx/MembershipGroupId = 0» (dans les guillemets doubles) à la fin de l’URL du site. 

Exemple: https://< «contoso» >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Sélectionnez l’utilisateur dans la liste.

- Cliquez sur **Supprimer les autorisations des utilisateurs** du ruban. 
-  Rajoutez l’utilisateur et renvoyez-le à l’utilisateur.

