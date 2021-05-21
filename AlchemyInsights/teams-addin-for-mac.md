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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582068"
---
# <a name="teams-add-in-for-mac"></a>Complément Teams pour Mac

Pour résoudre les problèmes liés à l’absence d’un complément Teams pour Mac, procédez comme suit :

**Étape 1 :** si vous avez un environnement Exchange hybride (2016 CU3 ou version ultérieure requise), utilisez l’outil Test-HMA.ps1 pour confirmer que l’authentification moderne hybride est correctement configurée. Pour plus d’informations, consultez [Validation de la configuration de l’authentification moderne hybride pour Outlook pour iOS et Android](https://aka.ms/TestHMAEAS).  

**Remarque** utiliser le format d’adresse UPN (par exemple, [username@contoso.com](mailto:username@contoso.com)), et non domaine\nomutilisateur. Pour ce faire, même pour les utilisateurs disposant de boîtes aux lettres Exchange Online.

**Étape 2 :** demander à l’utilisateur d’accéder à **outils** > **Comptes**... dans Outlook pour Mac, recherchez et sélectionnez le compte. Vérifiez que le nom d’utilisateur indiqué est au format UPN (par exemple, [username@contoso.com](mailto:username@contoso.com)).

**Étape 3 :** confirmer que l’utilisateur est titulaire d’une licence Microsoft Teams. L’utilisateur doit utiliser l’abonnement Office 365 pour Mac, le produit 16.24 ou version ultérieure.