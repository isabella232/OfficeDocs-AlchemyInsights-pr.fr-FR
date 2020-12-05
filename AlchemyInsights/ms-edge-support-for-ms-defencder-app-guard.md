---
title: Prise en charge de Microsoft Edge pour Microsoft Defender application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576546"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Prise en charge de Microsoft Edge pour Microsoft Defender application Guard

Conçu pour Windows 10 et Microsoft Edge, application Guard utilise une approche d’isolation matérielle qui permet à un utilisateur de naviguer dans un site non approuvé depuis un conteneur isolé Hyper-V, séparé du système d’exploitation hôte.

Un administrateur d’entreprise définit une liste de sites Web approuvés, de ressources Cloud et de réseaux internes. Lorsqu’un utilisateur visite un site qui ne figure pas dans la liste, Microsoft Edge ouvre le site dans le conteneur. Cela signifie que si le site s’avère malveillant, le PC hôte restera protégé et l’agresseur n’obtiendra pas les données de l’entreprise.

L’installation des extensions dans le conteneur est prise en charge à partir de la version 81 de Microsoft Edge et elle peut être contrôlée via une stratégie. L’adresse updateURL qui est utilisée dans la stratégie ExtensionInstallForcelist doit être ajoutée en tant que ressource neutre dans les stratégies d’isolation réseau utilisées par application Guard.

Pour plus d’informations, consultez la rubrique [prise en charge de Microsoft Edge pour Microsoft Defender application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
