---
title: how-to-import-nk2-files
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
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043204"
---
# <a name="how-to-import-nk2-files"></a>Comment importer des fichiers .nk2 

Lorsque vous démarrez Microsoft Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook pour Microsoft 365 pour la première fois, votre cache de surnoms (stocké dans le fichier .nk2 *profilename)* est importé dans un message masqué dans votre magasin de messages par défaut.

Pour importer des fichiers .nk2 dans Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook pour Microsoft 365, assurez-vous que le fichier .nk2 se trouve dans le dossier suivant : %appdata%\Microsoft\Outlook

**Remarque**: le fichier .nk2 doit avoir le même nom que votre profil Outlook 2013 ou Outlook 2016 actuel. Par défaut, le nom du profil est « Outlook ». Pour vérifier le nom du profil, suivez les étapes suivantes : 
1. Cliquez sur **Démarrer**, puis sur **Panneau de configuration**.
2. Double-cliquez sur **Courrier**.
3. Dans la boîte de dialogue Configuration du courrier, **sélectionnez Afficher les profils.**
4. Sélectionnez **Démarrer** > **Exécuter**.
5. Dans la **zone Ouvrir,** *tapezoutlook.exe /importnk2,* puis sélectionnez **OK.** 

Après avoir importé le fichier .nk2, son contenu est fusionné dans le cache de surnoms existant stocké dans votre boîte aux lettres.

Remarque : le fichier .nk2 est renommé avec une extension de nom de fichier .old lors du prochain démarrage de Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook pour Microsoft 365. Si vous souhaitez ré-importer le fichier .nk2, supprimez d’abord l’extension de nom de fichier .old.

Pour plus d’informations, voir Importer ou copier la liste de mise à jour automatique [sur un autre ordinateur.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)