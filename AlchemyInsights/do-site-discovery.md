---
title: Effectuer une détection du site
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 5ae99192c769dd5d5acae1c6e8f9b021e824b465
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322165"
---
# <a name="do-site-discovery"></a>Effectuer une détection du site

Si votre organisation utilise toujours des applications web héritées et envisage utiliser le mode Internet Explorer (ce que la plupart des clients font), vous devez découvrir davantage de sites.

**Vous avez déjà déployé une version antérieure de Microsoft Edge**

Si vous avez déjà configuré votre liste de sites d’entreprise pour qu’elle fonctionne avec la version héritée de Microsoft Edge, votre découverte de sites est alors quasiment terminé. Il vous suffit d’ajouter des sites neutres.

Les sites neutres sont généralement des sites qui fournissent une authentification unique (SSO). Si vous accédez à un site neutre à partir de Microsoft Edge, l’authentification se fera dans Microsoft Edge. Si vous accédez à un site neutre en mode Internet Explorer, l’authentification se fera en mode internet Explorer.

Identifiez les sites SSO ou autres sites neutres que vous utilisez et ajoutez-les à votre liste de sites d’entreprise.

**Internet Explorer est votre navigateur par défaut.**

Si vous avez commencé à utiliser Internet Explorer récemment, il est probable que vous ne sachiez pas les sites mis au niveau de sites web modernes mais qui exigent encore Internet Explorer. Vous devez rechercher et ajouter ces sites à la liste des sites d’entreprise, afin d’utiliser Internet Explorer pour ces uniquement.

**Remarque**: [Entreprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) découvre les sites qui pourraient nécessiter le mode Internet Explorer. Il y a la possibilité de collecter des données sur les ordinateurs exécutant Windows Internet Explorer 8 à 11 sur Windows 10, Windows 8.1, ou Windows 7.

**Analyser les données**

Une fois que vous avez collecté les données de site, nous recommandons d’utiliser cette procédure à 4 étapes pour analyser les données :
1. Triez les données par domaine, puis par URL.
2. Définissez les limites d’une « application » à configurer en mode Internet Explorer. Vous voulez inclure tous les sites et contrôles web qui définissent l’application, mais vous ne voulez pas inclure des sites et contrôles supplémentaires. Certains sites peuvent être aussi simples que *https://contoso.com/app1*, tandis que d’autres pourraient nécessiter la définition de plusieurs sites et pages.
3. Testez l’application pour vérifier qu’elle ne fonctionne pas en mode natif. De nombreux sites proposent du contenu moderne lorsqu’ils détectent un navigateur moderne et proposent uniquement du contenu hérité lorsqu’ils détectent Internet Explorer.
4. Ajoutez l’application à votre liste de sites d’entreprise en cas d’échec du test.

**Remarque**: pour une meilleure pratique, il est recommandé de regrouper tous les sites qui composent une application. Ainsi, lorsque vous mettez à niveau une application, il est plus facile de supprimer l’intégralité du site du mode Internet Explorer et de commencer à utiliser un navigateur moderne pour cette application.

Une fois que vous avez terminé la découverte de site et que vous avez analysé les données, vous pouvez  commencer à regarder la stratégie de canal.

