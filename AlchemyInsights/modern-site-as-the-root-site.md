---
title: Site moderne en tant que site racine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000390"
---
# <a name="modern-site-as-root-site"></a>Site moderne en tant que site racine

Nous avons commencé à déployer une nouvelle fonctionnalité qui vous permettra d’échanger votre site racine de site classique [avec un site moderne.](https://docs.microsoft.com/sharepoint/modern-root-site) Utilisez [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site avec un autre site lors de l’archivage du site d’origine. Disponible pour site d’équipe (non connecté à un groupe) et Site de communication.

>[!Important]
> Ne supprimez pas votre site racine classique pour créer un site de communication moderne. Cette situation n’est pas prise en charge par Microsoft. La suppression du site racine rend tous les sites SharePoint de votre organisation inaccessibles à tous les utilisateurs, jusqu’à ce que vous restyiez le site ou que vous en créez un à la même URL. Nous communiquerons cette fonctionnalité via le centre de messages. Vous devez vous attendre à ce que la fonctionnalité soit bientôt allumée dans votre client.

## <a name="known-issues-with-swapping-sites"></a>Problèmes connus avec l’échange de sites
- Le site cible peut renvoyer une erreur « in trouvée » (HTTP 404) pendant une courte période.
- Le contenu doit être réaxé pour mettre à jour l’index de recherche. Aucune étape manuelle n’est requise ici, cette étape est effectuée automatiquement.
- Tout ce qui dépend des liens « statiques » (tels que la synchronisation de fichiers et OneNote fichiers) doit être corrigé manuellement.
- Project Les sites serveur devront peut-être être validés pour s’assurer qu’ils sont toujours associés correctement. 
