---
title: L’utilisateur reçoit l’erreur AADSTS7000112 Yammer est désactivé
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796646"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>L’utilisateur reçoit l’erreur AADSTS7000112 Yammer est désactivé

Si le message d’erreur « AADSTS7000112 : L’application '00000005-0000-0ff1-CE00-000000000000'(Yammer) est désactivée » s’affiche, cela indique qu’il existe un problème avec le principal de service dans Azure AD. Un administrateur a peut-être désactivé le principal de service pour bloquer l’accès à Yammer.

La désactivation du principal de service n’est pas recommandée et peut entraîner d’autres problèmes. Pour plus d’informations sur l’approche prise en charge pour bloquer l’accès des utilisateurs à Yammer, voir [Désactiver l’accès à Yammer pour les utilisateurs de Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Pour résoudre ce problème dans le portail Azure et restaurer l’accès des utilisateurs à Yammer :

1.  Ouvrez la page Azure Active Directory, puis sélectionnez **Applications d’entreprise** sous **Gérer** dans le volet de navigation gauche.
3.  Tapez **Office 365 Yammer** dans la zone de recherche, puis sélectionnez le nom de l’application pour ouvrir les paramètres.
4.  Sélectionnez **Propriétés** sous **Gérer** dans le volet de navigation gauche.
5.  Définissez la valeur de **Activé pour que les utilisateurs se connectent ?** sur **Oui**, puis sélectionnez **Enregistrer**.
6.  Reconnectez-vous à Yammer. Il se peut que vous deviez effacer les cookies.

Vous pouvez également exécuter les commandes PowerShell pour définir la valeur. Pour plus d’informations, voir [Erreur « Désolé, nous n'avons pas pu vous connecter. » lorsque vous cliquez sur la vignette Yammer dans Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 