---
title: Modifier les canaux de mise à jour pour les applications Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 70b416e2b572fe9b4257648e3426b4d36975681e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756497"
---
# <a name="change-update-channels-for-office-apps"></a>Modifier les canaux de mise à jour pour les applications Office

Pour les nouvelles installations Office, utilisez les paramètres de téléchargement du logiciel Office pour sélectionner le canal de mise à jour souhaité, puis installez (ou réinstallez) les applications Office. Pour plus d’informations, consultez [Gérer les paramètres de téléchargement des logiciels dans Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Remarque** le canal de mise à jour sélectionné à l’aide des paramètres de téléchargement du logiciel Office s’applique à tous les utilisateurs effectuant de nouvelles installations à l’aide du Portail Office 365. Pour plus d’informations, consultez [Télécharger et installer ou réinstaller Microsoft 365 ou Office 2019 sur un PC ou Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Pour les installations Office existantes, utilisez l’outil Déploiement d’Office (ODT) pour basculer vers un autre canal de mise à jour :  

1. Téléchargez la dernière version de l’outil de Déploiement d’Office (setup.exe) à partir du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifiez le nom du canal vers lequel vous voulez basculer. Pour plus d’informations, consultez [Options de configuration pour l’outil déploiement d’Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Créez un fichier XML de configuration spécifiant le nom du canal approprié (par exemple, update.xml).  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. À partir d’une invite de commandes avec élévation de privilèges, basculez vers l’emplacement du dossier où setup.exe réside et exécutez la commande suivante :  
    a. setup.exe /configurer update.xml
5. Lancez une application Office (par exemple, Excel), puis sélectionnez **Fichier** > **Compte**. Dans la section Informations sur le produit, sélectionnez **Options de mise à jour** > **Mettre à jour**.

Pour plus d’informations, consultez [Comment changer les canaux de mise à jour des applications Office existantes](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Pour changer les canaux de mise à jour pour un groupe d’utilisateurs sélectionné ou à l’aide de Gestionnaire de configuration (SCCM), configurez le paramètre de canal de mise à jour à l’aide de GPO. Si vous souhaitez pour plus d’informations, consultez la rubrique relative à la [Présentation des canaux de mise à jour pour Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Pour plus d’informations, consultez les rubriques [Comment gérer les canaux Office 365 ProPlus pour les professionnels de l’informatique](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) et [Gérer les mises à jour vers Microsoft 365 Apps avec Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).