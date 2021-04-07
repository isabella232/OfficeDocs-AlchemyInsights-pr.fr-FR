---
title: Installer Office et OneDrive sur Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590273"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installer Office et OneDrive sur Windows Virtual Desktop

1. [Préparer et personnaliser une image VHD maître](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Créez une machine virtuelle (VM) si elle n'a pas encore été créée.

1. [Installer Office en mode d'activation sur ordinateur partagé](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). L'activation d'un ordinateur partagé permet à plusieurs utilisateurs d'accéder à Office.

1. [Installer OneDrive en mode par machine](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalement, OneDrive est installé par utilisateur, mais ici, il devrait être installé par machine.