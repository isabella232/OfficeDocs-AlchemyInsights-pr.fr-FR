---
title: Site moderne comme site racine
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666868"
---
# <a name="modern-site-as-root-site"></a>Site moderne en tant que site racine

Nous avons commencé à déployer une nouvelle fonctionnalité qui vous permettra d' [échanger votre site racine de site classique à l’aide d’un site moderne](https://docs.microsoft.com/sharepoint/modern-root-site). Utilisez [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site sur un autre site lors de l’archivage du site d’origine. Disponible pour les deux sites d’équipe (non connecté à un groupe) et le site de communication.

>[!Important]
> Ne supprimez pas votre site racine classique pour créer un site de communication moderne. Ceci n’est pas pris en charge par Microsoft. La suppression du site racine rendra tous les sites SharePoint de votre organisation inaccessibles à tous les utilisateurs, jusqu’à ce que vous restauriez le site ou que vous créez un nouveau site à la même URL. Nous communiquerons cette fonctionnalité via le centre de messages. Attendez-vous à ce que la fonctionnalité soit activée dans votre client.

## <a name="known-issues-with-swapping-sites"></a>Problèmes connus liés à l’échange de sites
- Le site cible peut renvoyer une erreur « introuvable » (HTTP 404) pendant une courte période de temps.
- Le contenu doit être réanalysé pour mettre à jour l’index de recherche. Il n’y a pas d’étape manuelle requise ici, cette opération sera exécutée automatiquement.
- Tout ce qui dépend de liens « statiques » (tels que la synchronisation de fichiers et les fichiers OneNote) doit être corrigé manuellement.
- Les sites Project Server peuvent avoir besoin d’être validés pour s’assurer qu’ils sont toujours correctement associés. 
