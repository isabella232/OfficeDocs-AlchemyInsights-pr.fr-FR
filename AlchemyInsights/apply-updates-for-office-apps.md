---
title: Appliquer les mises à jour pour les applications Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969383"
---
# <a name="apply-updates-for-office-apps"></a>Appliquer les mises à jour pour les applications Office

Par défaut, les mises à jour des applications Office sont gratuites, téléchargées automatiquement et appliquées en arrière-plan, sans aucune intervention de l’utilisateur. Pour exécuter les mises à jour manuellement si vous rencontrez des problèmes lors de l’application des mises à jour, consultez [Installer les mises à jour d’Office](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5). Pour plus d’informations, consultez [Résoudre les problèmes d’installation d’Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

Pour gérer les mises à jour d’Office pour vos utilisateurs, considérez les options suivantes :

- Sélectionnez le canal de mise à jour Office approprié pour votre organisation sur la base de la fréquence de mise à jour souhaitée. Pour plus d’informations, consultez la rubrique relative à la [Présentation des canaux de mise à jour pour Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).

- Décidez si vous voulez appliquer les mises à jour automatiquement à partir d’Internet ou à partir d’un partage local. Pour savoir comment procéder, consultez [Comment gérer les mises à jour apportées à Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).

- Consultez les paramètres de mise à jour d’Office pour contrôler la manière dont les mises à jour sont appliquées aux ordinateurs des utilisateurs finaux :

    - [Définir les paramètres de mise à jour pour Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [Définir la façon dont Office est mis à jour après l’installation](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).

Lorsque vous déployez des applications Office auprès de plusieurs utilisateurs, utilisez l’outil de personnalisation Office pour créer des fichiers de configuration pour le déploiement et configurer les mises à jour d’Office à l’aide de l’outil déploiement d’Office. Pour plus de détails, consultez [Vue d’ensemble de l’Outil de personnalisation Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) et l’[Outil de personnalisation Office](https://go.microsoft.com/fwlink/p/?LinkID=626065).

- Pour consulter un exemple de configuration des groupes d’utilisateurs pour déployer les mises à jour d’Office, consultez [Déploiement Microsoft 365 Apps à partir d’une source locale](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).
-   Pensez à utiliser le paramètre ForceAppShutdown au cas où les mises à jour de l'Office ne seraient pas appliquées à quelques utilisateurs en raison de l'ouverture des applications de l'Office. Pour plus d’informations, consultez la [Propriété FORCEAPPSHUTDOWN (partie de l’élément Property)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element) 

**Voir aussi**

[Présentation de la procédure de mise à jour de Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Informations sur la publication des mises à jour de Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).  
[Gérer les mises à jour vers Microsoft 365 Apps avec Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).  
