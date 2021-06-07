---
title: 1048 5.7.750 Service indisponible. Client bloqué pour l’envoi à partir de domaines non enregistrés
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774249"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>Client 5.7.750 interdit d’envoi à partir d’un domaine non enregistré

L’erreur se produit lorsqu’un grand nombre de messages sont envoyés à partir de domaines qui ne sont pas provisionn s dans votre client (ajoutés en tant que domaines acceptés et validés).

Pour éviter cette erreur, vous pouvez utiliser un connecteur de flux de messagerie basé sur un certificat dans lequel le domaine du certificat est un domaine provisionnable, ou vous pouvez mettre en service tous les domaines d’envoi.

Pour plus d’informations, voir [Corriger les problèmes de remise des e-mails pour les codes d’erreur 5.7.700 à 5.7.750 dans Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).