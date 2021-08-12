---
title: Permutation de votre site racine classique avec un site moderne
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940817"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Permutation de votre site racine classique avec un site moderne

Si votre environnement a été installé avant avril 2019, vous pouvez modifier votre site racine en site moderne à l’aide de Microsoft PowerShell :

- Si vous avez un autre site que vous souhaitez utiliser comme site racine, vous pouvez remplacer [(permuter)](https://docs.microsoft.com/sharepoint/modern-root-site) le site racine par celui-ci. 
    - Utilisez [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site avec un autre site lors de l’archivage du site d’origine. Disponible pour site d’équipe (non connecté à un groupe) et Site de communication. 

- Des fonctionnalités supplémentaires seront bientôt introduites pour vous permettre de continuer à utiliser le contenu du site, mais de convertir le site existant en site de communication. 
>[!Important]
>Ces fonctionnalités seront déployées progressivement. Continuez à vérifier les mises à jour dans le Centre de messages. 

## <a name="known-issues-with-swapping-sites"></a>Problèmes connus avec l’échange de sites

- Le site cible peut renvoyer une erreur « in trouvée » (HTTP 404) pendant une courte période.
- Le contenu doit être réaxé pour mettre à jour l’index de recherche. Aucune étape manuelle n’est requise : cette étape est effectuée automatiquement.
- Tout ce qui dépend des liens « statiques » (tels que la synchronisation de fichiers et OneNote fichiers) doit être corrigé manuellement.
- Si le site source était un site d’actualités de l’organisation, mettez à jour l’URL. Obtenir la liste de tous les sites d’actualités de l’organisation.
- Project Les sites serveur devront peut-être être validés pour s’assurer qu’ils sont toujours associés correctement.
