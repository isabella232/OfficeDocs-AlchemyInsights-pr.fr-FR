---
title: procédure-Import-NK2-Files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780057"
---
# <a name="how-to-import-nk2-files"></a>Procédure d’importation de fichiers. NK2 

Lorsque vous démarrez Microsoft Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook pour Microsoft 365 pour la première fois, votre cache des surnoms (stocké dans le fichier *ProfileName*. NK2) est importé dans un message masqué dans votre banque de messages par défaut.

Pour importer des fichiers. nk2 dans Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook pour Microsoft 365, assurez-vous que le fichier. nk2 se trouve dans le dossier suivant :%appdata%\Microsoft\Outlook

**Remarque**: le fichier. nk2 doit porter le même nom que votre profil Outlook 2013 ou Outlook 2016 actuel. Par défaut, le nom du profil est « Outlook ». Pour vérifier le nom du profil, procédez comme suit : 
1. Cliquez sur **Démarrer**, puis sur **Panneau de configuration**.
2. Double-cliquez sur **courrier**.
3. Dans la boîte de dialogue Configuration de la messagerie, sélectionnez **afficher les profils**.
4. Sélectionnez **Démarrer**l'  >  **exécution**.
5. Dans la zone **ouvrir** , tapez *outlook.exe/importnk2*, puis sélectionnez **OK**. 

Après avoir importé le fichier. nk2, le contenu du fichier est fusionné dans le cache de surnoms existant stocké dans votre boîte aux lettres.

**Remarque**: le fichier. nk2 est renommé avec l’extension de nom de fichier. Old la prochaine fois que vous démarrez Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook pour Microsoft 365. Si vous souhaitez réimporter le fichier. nk2, supprimez d’abord l’extension de nom de fichier. old.

Pour plus d’informations, reportez-vous [à la rubrique importer ou copier la liste de saisie semi-automatique sur un autre ordinateur](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).