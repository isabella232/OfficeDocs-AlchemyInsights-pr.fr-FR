---
title: Configuration virtuelle avec les services de domaine AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884580"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Configuration virtuelle avec les services de domaine AAD

La configuration virtuelle avec les services de domaine AAD comprend ces étapes : 

1. La vérification de l’intégrité de votre domaine sur le portail Azure https://aka.ms/aadds-health
2. La recherche dans votre NSG des règles qui bloquent les ports nécessaires à la synchronisation dans les services de domaine Azure AD sur le portail https://aka.ms/aadds-networking
3. Vous assurer que votre réseau virtuel est déployé dans la même région Azure que le domaine géré par les services de domaine Azure AD.
4. Vous assurer que vous n’avez pas de domaine existant avec le même nom de domaine disponible sur le réseau virtuel.

Pour plus d’informations sur les considérations en matière de conception sur Réseau Virtuel Azure afin de prendre en charge les services de domaine AAD, consultez[Considération du Réseau Virtuel](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

