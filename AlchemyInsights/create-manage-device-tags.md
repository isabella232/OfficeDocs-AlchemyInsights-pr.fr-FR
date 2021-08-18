---
title: Créer et gérer des balises ou des groupes d’appareils
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: c06ed00d7cf4bcb23fdcee12f446953918075728
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325647"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Créer et gérer des balises ou des groupes d’appareils

Ajoutez des balises sur les appareils pour créer une affiliation de groupe logique. Les balises d’appareil prennent en charge le mappage approprié du réseau, ce qui vous permet d’attacher différentes balises pour capturer le contexte et d’activer la création de liste dynamique dans le cadre d’un incident. Les balises peuvent être utilisées comme filtre dans l’affichage Liste des appareils ou pour regrouper des appareils. Pour plus d’informations sur le regroupement d’appareils, consultez [Créer et gérer des balises d’appareil](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags).

Vous pouvez ajouter des balises sur les appareils en :

- Utilisation du portail

- Définition d’une valeur de clé de Registre
 
**Remarque :** Il peut y avoir une latence entre le moment où une balise est ajoutée à un appareil et sa disponibilité dans la liste des appareils et la page de l’appareil.

Pour ajouter des balises d’appareil à l’aide de l’API, consultez [Ajouter ou supprimer des balises d’appareil API](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Ajouter et gérer des balises d’appareil à l’aide du portail

1. Sélectionnez l’appareil sur lequel vous souhaitez gérer les balises. Vous pouvez sélectionner ou rechercher un appareil à partir de l’une des vues suivantes :

    - **Tableau de bord des opérations de sécurité** Sélectionnez le nom de l’appareil dans la section Principaux appareils associés à des alertes actives.
    - **File d’attente des alertes** : sélectionnez le nom de l’appareil en regard de l’icône de l’appareil dans la file d’attente des alertes.
    - **Liste des appareils** : sélectionnez le nom de l’appareil dans la liste des appareils.
    - **Zone de recherche** : sélectionnez Appareil dans le menu déroulant et entrez le nom de l’appareil.

    Vous pouvez également accéder à la page d’alerte via les Affichages de fichier et d’adresse IP.

1. Sélectionnez **Gérer les balises** dans la ligne des actions de réponse.

1. Taper pour rechercher ou créer des balises.

Les balises sont ajoutées à la vue appareil et sont répercutées dans l’affichage Liste des appareils. Vous pouvez ensuite utiliser le filtre Balises pour afficher la liste des appareils appropriés.

Pour plus d'informations, consultez la rubrique [Créer et gérer des balises d’appareil](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags).