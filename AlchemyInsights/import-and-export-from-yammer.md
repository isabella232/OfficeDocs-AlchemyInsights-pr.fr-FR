---
title: Importer et exporter à partir de Yammer
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
- "9735"
- "9003224"
ms.openlocfilehash: 3ead2702c2fbd26b2e5596e26e9189c2f97baf93c93ec3cbd57f15c855b5128e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54001470"
---
# <a name="import-and-export-from-yammer"></a>Importer et exporter à partir de Yammer

**Import**

Les options d’importation de l’utilisateur varient selon que votre réseau Yammer soit en [Mode natif pour Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ou non.

- **Mode non natif** : les utilisateurs peuvent être importés dans des groupes à l’aide de [Ajouter à partir du carnet d’adresses](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limite à 100 utilisateurs) au sein des paramètres de groupe, ou au réseau à l’aide de [Mise à jour en bloc](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) au sein de l’administrateur réseau.
- **Mode natif** : les opérations d’appartenance au groupe et d’appartenance au réseau doivent être effectuées à partir du [Portail d’administration Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [Portail Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ou à l’aide d’une autre option d’Azure AD. Les réseaux en mode natif n’ont plus accès à la mise à jour en bloc et à d’autres fonctionnalités héritées.

> [!IMPORTANT]
> Yammer n’a jamais pris en charge l’importation de contenu à partir d’un administrateur réseau même lorsque la fonctionnalité d’exportation de données était utilisée dans un autre réseau. Le contenu peut être publié de nouveau par des solutions partenaires ou par les API Yammer REST.

**Exportation**

[L’exportation des données du réseau au sein de l’administrateur réseau](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permet d’exporter du contenu à partir de réseaux Yammer, y compris des messages et des fichiers. Les pièces jointes peuvent être extrêmement volumineuses et entraîner des délais d'exécution importants pour les exportations. Nous vous recommandons d’exporter des réseaux actifs à l’aide de l’[API d'exportation de données](https://developer.yammer.com/docs/data-export-api) par tranches de jours ou de semaines. Le Support Microsoft ne fournit pas de scripts personnalisés à cet effet.

Une [exportation GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) distincte existe pour exporter le contenu pour un utilisateur individuel.