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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968375"
---
# <a name="changing-ews-throttling-settings"></a>Modification des paramètres de limitation du service EWS

Exécutez nos tests automatisés pour vous permettre de modifier la stratégie de limitation du service EWS pour la durée de votre migration. Notez que, même une fois cette action exécuté, les importations EWS restent limitées à 150 Mo par 5 minutes par boîte aux lettres. Afin d’augmenter le débit de migration, migrez davantage d’utilisateurs simultanément.

Notez que les modifications apportées à la stratégie de limitation de l’application EWS n’ont aucun effet sur les types de migration suivants (à l’aide des outils Microsoft) : hybride, basculement/intermédiaire (RPC/HTTP), IMAP, G suite, dossier public ou service d’importation PST.