---
title: Expédition de disque dans le service d’importation Microsoft 365
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
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721691"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Expédition de disque dans le service d’importation Microsoft 365

Utilisez l’expédition de disque en copiant les fichiers PST sur un disque dur, puis en expédiant le disque dur à Microsoft.

Pour démarrer la tâche :

1. Dans le Centre de conformité Microsoft 365 sous **Gouvernance des informations**, sélectionnez **Importer**.

1. Sélectionnez **Choisir le type de tâche d’importation**, puis sélectionnez **Suivant**.

1. Pour afficher les étapes de cette option d’importation, sélectionnez **Expédier des disques durs à l’un de nos emplacements physiques**.

Voici quelques éléments à retenir :

- Le rôle Importation/Exportation de boîtes aux lettres doit vous avoir été attribué dans Exchange Online pour pouvoir importer des fichiers PST dans des boîtes aux lettres Microsoft 365.
Les performances peuvent être affectées pour les fichiers PST supérieurs à 20 Go.

- Seuls les lecteurs SSD 2,5 ou 2,5 pouces ou les disques durs internes 3,5 pouces SATA II/III sont pris en charge.
Le disque dur contenant des fichiers PST doit être chiffré avec BitLocker.

- Le tarif pour importer des fichiers PST dans les boîtes aux lettres Microsoft 365 via l’expédition de disque s’élève à 2 $ USD par Go de données.

Pour plus d’informations sur l’utilisation de la méthode d’expédition de lecteur pour importer des fichiers PST, consultez [Utiliser l’expédition de lecteur pour importer les fichiers PST de votre organisation](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).