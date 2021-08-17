---
title: L’inventaire logiciel est manquant ou incorrect
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: 191d6ae772dc1b1c6b15071da9c4aca14429cf2db17be6ee0db6b23ea0d29e2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084641"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>L’inventaire logiciel est manquant ou incorrect

L'inventaire des logiciels dans le cadre de la gestion des menaces et des vulnérabilités (GVT) est une liste des logiciels connus dans votre organisation avec les énumérations officielles de la plateforme commune (CPE).

Les produits logiciels sans CPE officielles n'ont pas de vulnérabilités publiées. L'inventaire comprend également des informations telles que le nom du fournisseur, le nombre de faiblesses, les menaces et le nombre d'appareils exposés.

Les modifications apportées aux logiciels sur les appareils sont généralement reflétées dans les portails de sécurité en moins de deux heures. Toutefois, cela peut parfois prendre plus de temps. Il est actuellement impossible de forcer une synchronisation ; il s'agit d'une évaluation continue.

Si vous avez apporté un changement de logiciel et que la modification n’est pas reflétée avec précision dans TVM après 5 heures, procédez comme suit :

1. Consultez la section sur les preuves du logiciel pour comprendre comment le logiciel a été détecté.
1. Assurez-vous que le logiciel est pris en charge. Le logiciel peut être visible uniquement au niveau de l’appareil, même s’il n’est actuellement pas pris en charge par la gestion des menaces et vulnérabilités. Toutefois, seules des données limitées sont disponibles.
1. Pour savoir comment signaler l’erreur d’accès à partir du portail, consultez [Signaler une inexactitude](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Remarque** : signaler une inexactitude à partir du portail MDE est un canal à sens unique vers l'ingénierie. Si le problème est urgent, ouvrez un ticket de support.

Pour plus d’informations, voir [Inventaire logiciel – gestion des menaces et des vulnérabilités](/microsoft-365/security/defender-endpoint/tvm-software-inventory).