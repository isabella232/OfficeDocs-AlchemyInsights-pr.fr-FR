---
title: Erreur d’atténuation de l’application non détectée
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666976"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Erreur d’atténuation « l’application non détectée »

L’erreur d’installation de l’application « l’application n’a pas été détectée une fois l’installation réussie », signalée par Intune, peut se produire sur toutes les plateformes de système d’exploitation principales (Windows, iOS et Android).

Les situations les plus courantes qui génèrent cette erreur sont les suivantes :

- L’application a été mise à jour en dehors de Intune (à partir d’un magasin d’applications tierce) après le déploiement initial. Par exemple, certaines applications telles que Google Chrome peuvent effectuer des mises à jour automatiques.
- Un utilisateur a désinstallé l’application après l’installation initiale.

Pour résoudre ce problème, vous devez commencer par réviser les appareils concernés afin de déterminer le scénario dans lequel l’erreur se produit.

- Si l’application a été mise à jour en dehors d’Intune, le déploiement de l’application peut être configuré pour ignorer la version de l’application. Pour ce faire, sous **Configuration de l’application > Informations sur l’application**, définir la version **Ignorer l’application** à **Oui**.
- Lorsque vous ciblez le client, il peut être utile de déployer l’application en tant que « obligatoire » et de s’assurer que la dernière version est déployée.
- Par ailleurs, sur la plateforme iOS, il est possible d’utiliser la fonctionnalité **autoupdate** associée au programme d’achat du volume Apple, qui peut être configuré pour effectuer une mise à jour automatique vers les nouvelles versions des applications dès qu’elles sont disponibles.

Pour plus d’informations sur la résolution des problèmes d’installation de l’application, consultez [Résoudre les problèmes d’installation d’application](https://docs.microsoft.com/intune/troubleshoot-app-install).
