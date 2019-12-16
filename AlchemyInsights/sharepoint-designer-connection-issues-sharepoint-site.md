---
title: Problèmes de connexion avec SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051711"
---
# <a name="sharepoint-designer-connection-issues"></a>Problèmes de connexion avec SharePoint Designer 

Si SharePoint Designer rencontre des problèmes de connexion aux sites SharePoint, essayez les solutions courantes suivantes.

Étape 1 : Vérifiez que SharePoint Designer 2013 est mis à jour avec [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) et la [mise à jour 2016 du 2 août pour SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Étape 2 : effacez les fichiers du cache local :

1. Fermez SharePoint Designer 2013.

2. Sur l’ordinateur local, supprimez tous les fichiers trouvés dans chacun des dossiers suivants.

    - %APPDATA%\Microsoft\Web serveur Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Ouvrez SharePoint Designer 2013 et entrez à nouveau le compte pour voir s’il fonctionne.

Étape 3 : [activez l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Étape 4 : les administrateurs devront **autoriser les scripts personnalisés** dans les paramètres du centre d’administration SharePoint pour autoriser la connexion à SharePoint Designer. Pour plus d’informations, reportez-vous à la rubrique [autoriser ou empêcher un script personnalisé](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


