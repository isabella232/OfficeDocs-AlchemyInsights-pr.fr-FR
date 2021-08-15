---
title: Problème avec l’attribut et le filtre d’étendue
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960185"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problème avec l’attribut et le filtre d’étendue

**Problème avec les valeurs UPN conflictuelles**

Le Workday pour l’approvisionnement d’utilisateurs AD affiche le message d’erreur **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. L’opération a échoué car la valeur UPN fournie pour l’ajout/modification n’est pas unique à l’échelle de la forêt. Détails de l’erreur : **CONSTRAINT_ATT_TYPE - userPrincipalName**.

La valeur **userPrincipalName** que le connecteur Workday tente de définir lors de la création du compte utilisateur AD existe déjà dans le domaine AD cible. Ceci implique que (1) l’utilisateur existe déjà et la vérification d’ID correspondante a échoué pour l’utilisateur ou (2) la règle de génération UPN a créé une valeur en conflit.

Voici les étapes de résolution suggérées :

Si l’utilisateur existe déjà et que l’ID correspondante n’a pas pu lier le compte Workday au compte Active Directory, vérifiez alors si l’attribut d’ID correspondant (généralement **employeeID**) dans Workday et AD correspond exactement. S’il n’existe pas de correspondance, il s’agit d’un problème nécessitant une correction. Par exemple, si l’EmployeeID est 001052 dans Workday et 1052 dans AD, le moteur d’approvisionnement ne pourra alors pas lier les deux comptes et tentera de créer un utilisateur qui existe déjà. La solution dans ce cas est de modifier la valeur **EmployeeID** dans AD pour inclure les zéros du début afin qu’elle soit 001052.
Si l’expression générant l’UPN ne créée pas de valeur unique, envisagez d’utiliser la fonction de déduplication **SelectUniqueValue** pour générer une valeur unique à chaque fois.

**Workday pour l’approvisionnement d’utilisateurs AD ne définit pas la valeur d’attribut manager pour le compte des utilisateurs AD**

La tâche Workday pour l’approvisionnement d’utilisateurs AD ne définit pas la valeur d’attribut **manager** pour les comptes des utilisateurs AD. Il existe deux scénarios possibles lorsque vous voyez ce comportement :

1. Le manager dans Workday ne peut pas être résolu dans un compte d’utilisateur AD correspondant car le manager ne se trouve pas dans l’étendue.
2. Dans un scénario de **domaines AD multiples**, le manager dans Workday n’est pas présent dans le même domaine que celui de l’utilisateur.

Pour résoudre le problème, essayez les étapes suivantes :

1. Si vous avez défini des filtres d’étendue, vérifiez d’abord que le manager est dans l’étendue et qu’il satisfait la clause d’étendue. Si le manager ne satisfait pas le filtre d’étendue, modifiez le filtre, de sorte que le manage se trouve également dans l’étendue de l’opération d’approvisionnement.
2. Si vous disposez de domaines AD multiples, le connecteur a donc une limitation connue d’incapacité à résoudre les références manager inter-domaines.

Pour d’autres détails sur la configuration de Workday pour l’approvisionnement automatique, voir [Tutoriel : Configurer Workday pour l'approvisionnement automatique d'utilisateurs](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













