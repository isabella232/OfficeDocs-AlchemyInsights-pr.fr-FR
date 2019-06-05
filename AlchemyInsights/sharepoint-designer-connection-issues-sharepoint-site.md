---
title: Niveaux d’autorisation SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716890"
---
# <a name="sharepoint-designer-connection-issues"></a>Problèmes de connexion avec SharePoint Designer 

<p>Si SharePoint Designer rencontre des problèmes de connexion aux sites SharePoint, essayez les solutions courantes suivantes.</p> <p><strong>Étape 1:</strong> <strong>Vérifier que SharePoint Designer est&nbsp; mis à jour</strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Mise à jour pour SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Étape 2:</strong> <strong>Effacer les fichiers du cache local</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Fermez SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Sur l’ordinateur local, accédez aux dossiers suivants pour supprimer les fichiers mis en cache.&nbsp;</li> <li style="font-weight: 400;">Cliquez sur <strong>Démarrer&gt; -exécuter</strong> et supprimez tous les fichiers trouvés sous chacun des emplacements ci-dessous.&nbsp;<br /><br />%APPDATA%\Microsoft\Web serveur Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Ouvrez SharePoint Designer 2013 et entrez à nouveau le compte pour voir s’il fonctionne.</li> </ol> <p><strong>Étape 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Activer l’authentification moderne pour Office 2013 sur les appareils Windows</strong></a>&nbsp;</p> <p><strong>Étape 4:</strong> Les <strong>administrateurs devront autoriser le script personnalisé à autoriser la connexion à SharePoint Designer</strong>.</p> <p>Pour obtenir la procédure détaillée, des exemples et des considérations, voir <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">autoriser ou empêcher les scripts personnalisés</a>.&nbsp;</p>


