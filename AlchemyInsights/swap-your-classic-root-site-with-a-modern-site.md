---
title: Échangez votre site racine classique avec un site moderne
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042925"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Échangez votre site racine classique avec un site moderne

Si votre environnement a été configuré avant le 2019 avril, vous pouvez remplacer votre site racine par un site moderne à l’aide de Microsoft PowerShell :

- Si vous souhaitez utiliser un autre site que celui de votre site racine, vous pouvez remplacer (remplacer [) le site racine](https://docs.microsoft.com/sharepoint/modern-root-site) par celui-ci. 
    - Utilisez [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site sur un autre site lors de l’archivage du site d’origine. Disponible pour les deux sites d’équipe (non connecté à un groupe) et le site de communication. 

- Des fonctionnalités supplémentaires seront bientôt introduites, qui vous permettront de continuer à utiliser le contenu sur le site, mais convertissez le site existant en un site de communication. 
>[!Important]
>Ces fonctionnalités seront déployées graduellement. Continuez à consulter le centre de messages Office 365 pour les mises à jour. 

## <a name="known-issues-with-swapping-sites"></a>Problèmes connus liés à l’échange de sites

- Le site cible peut renvoyer une erreur « introuvable » (HTTP 404) pendant une courte période de temps.
- Le contenu doit être réanalysé pour mettre à jour l’index de recherche. Aucune étape manuelle n’est requise : cette opération sera automatique.
- Tout ce qui dépend de liens « statiques » (tels que la synchronisation de fichiers et les fichiers OneNote) doit être corrigé manuellement.
- Si le site source était un site de News de l’organisation, mettez à jour l’URL.Obtenir la liste de tous les sites d’actualité de l’organisation.
- Les sites Project Server peuvent avoir besoin d’être validés pour s’assurer qu’ils sont toujours correctement associés.





