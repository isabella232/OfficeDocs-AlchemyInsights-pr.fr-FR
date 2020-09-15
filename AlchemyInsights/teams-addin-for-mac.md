---
title: Complément Teams pour Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670326"
---
# <a name="teams-add-in-for-mac"></a>Complément Teams pour Mac

Pour résoudre les problèmes liés à l’absence d’un complément Teams pour Mac, procédez comme suit :

**Étape 1 :** si vous avez un environnement Exchange hybride (2016 CU3 ou version ultérieure requise), utilisez l’outil Test-HMA.ps1 pour confirmer que l’authentification moderne hybride est correctement configurée. Pour plus d’informations, consultez [Validation de la configuration de l’authentification moderne hybride pour Outlook pour iOS et Android](https://aka.ms/AA980zq).  

**Remarque** utiliser le format d’adresse UPN (par exemple, [username@contoso.com](mailto:username@contoso.com)), et non domaine\nomutilisateur. Pour ce faire, même pour les utilisateurs disposant de boîtes aux lettres Exchange Online.

**Étape 2 :** demander à l’utilisateur d’accéder à **outils** > **Comptes**... dans Outlook pour Mac, recherchez et sélectionnez le compte. Vérifiez que le nom d’utilisateur indiqué est au format UPN (par exemple, [username@contoso.com](mailto:username@contoso.com)).

**Étape 3 :** confirmer que l’utilisateur est titulaire d’une licence Microsoft Teams. L’utilisateur doit utiliser l’abonnement Office 365 pour Mac, le produit 16.24 ou version ultérieure.