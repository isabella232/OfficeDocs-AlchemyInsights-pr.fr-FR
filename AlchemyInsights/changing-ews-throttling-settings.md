---
title: Modification des paramètres de limitation du service EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818034"
---
# <a name="changing-ews-throttling-settings"></a>Modification des paramètres de limitation du service EWS

Exécutez nos tests automatisés pour vous permettre de modifier la stratégie de limitation du service EWS pour la durée de votre migration. Notez que, même une fois cette action exécuté, les importations EWS restent limitées à 150 Mo par 5 minutes par boîte aux lettres. Afin d’augmenter le débit de migration, migrez davantage d’utilisateurs simultanément.

Notez que les modifications apportées à la stratégie de limitation de l’application EWS n’ont aucun effet sur les types de migration suivants (à l’aide des outils Microsoft) : hybride, basculement/intermédiaire (RPC/HTTP), IMAP, G suite, dossier public ou service d’importation PST.