---
title: SharePoint Problèmes de connexion du concepteur
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942023"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problèmes de connexion du concepteur 

Si SharePoint designer rencontre des problèmes de connexion à SharePoint sites web, essayez les solutions courantes suivantes.

Étape 1 : vérifiez que SharePoint Designer 2013 est mis à jour avec [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) et la mise à jour du 2 août [2016 pour SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Étape 2 : Effacer les fichiers de cache locaux :

1. Fermez SharePoint Designer 2013.

2. Sur l’ordinateur local, supprimez tous les fichiers trouvés dans chacun des dossiers suivants.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Ouvrez SharePoint Designer 2013 et entrez à nouveau le compte pour voir s’il fonctionne.

Étape 3 : Activer [l’authentification moderne Office 2013 sur Windows appareils mobiles.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Étape 4 : les  administrateurs doivent autoriser les scripts personnalisés dans les paramètres du SharePoint Admin Center pour autoriser la connexion SharePoint Designer. Pour plus [d’informations, voir](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) Autoriser ou empêcher les scripts personnalisés.


