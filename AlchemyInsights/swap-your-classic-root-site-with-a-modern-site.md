---
title: Échangez votre site racine classique avec un site moderne
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691177"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Échangez votre site racine classique avec un site moderne

Si votre environnement a été configuré avant le 2019 avril, vous pouvez remplacer votre site racine par un site moderne à l’aide de Microsoft PowerShell :

- Si vous souhaitez utiliser un autre site que celui de votre site racine, vous pouvez remplacer (remplacer [) le site racine](https://docs.microsoft.com/sharepoint/modern-root-site) par celui-ci. 
    - Utilisez [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pour permuter l’emplacement d’un site sur un autre site lors de l’archivage du site d’origine. Disponible pour les deux sites d’équipe (non connecté à un groupe) et le site de communication. 

- Des fonctionnalités supplémentaires seront bientôt introduites, qui vous permettront de continuer à utiliser le contenu sur le site, mais convertissez le site existant en un site de communication. 
>[!Important]
>Ces fonctionnalités seront déployées graduellement. Continuez à vérifier le centre de messages pour les mises à jour. 

## <a name="known-issues-with-swapping-sites"></a>Problèmes connus liés à l’échange de sites

- Le site cible peut renvoyer une erreur « introuvable » (HTTP 404) pendant une courte période de temps.
- Le contenu doit être réanalysé pour mettre à jour l’index de recherche. Aucune étape manuelle n’est requise : cette opération sera automatique.
- Tout ce qui dépend de liens « statiques » (tels que la synchronisation de fichiers et les fichiers OneNote) doit être corrigé manuellement.
- Si le site source était un site de News de l’organisation, mettez à jour l’URL.Obtenir la liste de tous les sites d’actualité de l’organisation.
- Les sites Project Server peuvent avoir besoin d’être validés pour s’assurer qu’ils sont toujours correctement associés.
