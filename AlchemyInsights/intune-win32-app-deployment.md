---
title: Déploiement d’applications Win32 avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925883"
---
# <a name="intune-win32-app-deployment"></a>Déploiement d’applications Win32 avec Intune

Microsoft Intune autorise les applications Win32, y compris, mais non limitées aux applications MSI et .EXE à déployer sur les appareils Windows 10. Le mécanisme de déploiement utilisé nécessite que l’IME (Intune Management Extension) soit présente sur l’appareil cible. L’IME est installée automatiquement suite au ciblage d’un script PowerShell ou d’une application Win32 sur un utilisateur/appareil.

Il existe également une série de conditions préalables devant être remplies pour déployer les applications Win32, notamment :

- Plateformes prises en charge : Windows 10 version 1607 ou ultérieure (versions Entreprise, Pro et Éducation).
- Architecture non prise en charge : x86 et x64.
- Gestion des appareils : AAD joint et inscrit automatiquement (y compris les jointures de domaines hybrides et les stratégies de groupe inscrites automatiquement).
- Format du package d’application : fichier .**intunewin** préparé par l’[outil de préparation de contenu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Limites :
    - Taille maximale : 8 Go.
    - Architecture non prise en charge : ARM.

Consultez le document [Ajouter, attribuer et surveiller une application Win32 dans Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add) pour plus d’informations sur ces étapes.

Pour plus d’informations sur la résolution des problèmes de déploiement des applications sur Windows, notamment les applications Win32, suivez les documents suivants :

- [Résoudre les problèmes d’installation d’application](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Résoudre les problèmes liés aux applications Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)