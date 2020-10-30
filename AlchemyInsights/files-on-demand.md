---
title: Fichiers à la demande
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791292"
---
# <a name="configure-files-on-demand"></a>Configurer les fichiers à la demande

Les fichiers OneDrive à la demande nécessitent [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 ou ultérieure) ou Windows Server 2019 et OneDrive Build 17.3.7064.1005 ou version ultérieure.

La fonctionnalité Fichiers à la demande OneDrive vous permet d’accéder à vos fichiers dans OneDrive sans avoir à en télécharger la totalité et à utiliser l’espace de stockage de votre appareil.

Pour configurer les fichiers à la demande sur votre PC :

1. Sélectionnez l’icône de nuage **OneDrive** blanc ou bleu dans la zone de notification de la barre des tâches Windows. Sélectionnez l'icône d’engrenages **Aide & paramètres** > **Paramètres** .
2. Dans l’onglet **Paramètres** , cochez la case **Libérez de l’espace et téléchargez des fichiers lorsque vous avez besoin de les utiliser** .  

Vous pouvez également configurer les fichiers à la demande à l’aide du registre.

Si vous désactivez ce paramètre, les utilisateurs de Windows 10 ont le même comportement de synchronisation que les utilisateurs des versions précédentes de Windows et ne peuvent pas activer la fonctionnalité Fichiers à la demande. Si vous ne configurez pas ce paramètre, les utilisateurs peuvent activer la fonctionnalité Fichiers à la demande ou la désactiver.

Cette stratégie définit la valeur de la clé de Registre suivante sur 1. Désactiver cette stratégie définit la valeur de la clé de registre suivante sur 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Si vous l’option Fichiers à la demande n’apparaît pas dans l’onglet Paramètres, assurez-vous que le type de démarrage du service Pilote de filtrage de fichiers dans le cloud Windows est défini sur 2 (AUTO_START). Activer cette fonctionnalité définit la valeur de la clé de registre suivante sur 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`