---
title: Résoudre le problème-utilisateur introuvable dans l’annuaire
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054808"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Résoudre le problème-utilisateur introuvable dans l’annuaire

Si les utilisateurs reçoivent un message d’erreur indiquant que l’utilisateur est introuvable dans le répertoire, réessayez en indiquant que le type de problème est User not in Directory.

Vous pouvez effectuer les étapes suivantes pour résoudre le problème.

- Assurez-vous que le compte qui a accepté l’invitation électronique est le même compte que celui utilisé pour la connexion ultérieure. Assurez-vous que l’utilisateur utilise le même compte pour accepter l’invitation et se connecter au site. 

Pour plus d’informations, reportez-vous à la rubrique [gestion</a> des alias de votre compte Microsoft pour gérer la connexion à Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Accédez à chaque site (s) dans lequel l’utilisateur reçoit l’erreur. 

Ajoutez « /_layouts/15/People.aspx/MembershipGroupId = 0 » (dans les guillemets doubles) à la fin de l’URL du site. 

Exemple : https://< « contoso » >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Sélectionnez l’utilisateur dans la liste.

- Cliquez sur **Supprimer les autorisations des utilisateurs** du ruban. 
-  Rajoutez l’utilisateur et renvoyez-le à l’utilisateur.

