---
title: 'Résoudre le problème : utilisateur in trouvé dans l’annuaire'
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098168"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Résoudre le problème : utilisateur in trouvé dans l’annuaire

Si les utilisateurs reçoivent le message d’erreur « l’utilisateur est in retrouveable » dans l’annuaire, essayez à nouveau lorsque le type de problème est Utilisateur qui n’est pas dans l’annuaire.

Les étapes suivantes peuvent être effectuées pour résoudre le problème.

- Assurez-vous que le compte qui a accepté l’invitation par courrier électronique est le même que celui utilisé pour se connecter ultérieurement. Assurez-vous que l’utilisateur utilise le même compte pour accepter l’invitation et se connecter au site. 

Pour plus d’informations, voir Comment gérer les alias de votre compte Microsoft pour gérer les Microsoft 365 [ </a> connexion.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Accédez à chaque site dans lequel l’utilisateur reçoit l’erreur. 

Ajoutez « /_layouts/15/people.aspx/membershipgroupid=0 » (entre guillemets doubles) à la fin de l’URL du site. 

Exemple : https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Sélectionnez l’utilisateur dans la liste.

- Cliquez **sur Supprimer les autorisations utilisateur** du Ruban. 
-  Ajoutez de nouveau l’utilisateur et renvoyez l’invitation à l’utilisateur.

