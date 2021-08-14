---
title: Résoudre l’erreur de connexion Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953020"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Résoudre l’erreur de connexion Teams AADSTS9000411

Lorsque vous vous connectez à Microsoft Teams, le message d’erreur suivant peut s’afficher : **Désolé... Nous rencontrons des difficultés pour vous connecter à AADSTS9000411 : la demande n’est pas correctement mise en forme. Le paramètre « login_hint » est dupliqué.**

Pour résoudre ce problème, assurez-vous que vos clients Microsoft Teams sont mis à jour. Pour plus d’informations sur la mise à jour de votre client, voir [Mettre à jour Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Si vous ne pouvez pas mettre à jour votre client pour une raison quelconque, la déconnexion du client efface la plupart des données mises en cache. Toutefois, si vous rencontrez encore des problèmes après la fermeture et l’ouverture de session, quittez Teams et effacez le cache de votre client en procédant comme suit :
1. Fermez Microsoft Teams.
2. Accédez à :%appdata%\microsoft\teams et supprimez tous les fichiers.
3. Ouvrir Microsoft Teams de nouveau.
