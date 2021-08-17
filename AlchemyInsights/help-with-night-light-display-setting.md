---
title: Aide sur le paramètre d’affichage en mode clair de nuit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078722"
---
# <a name="help-with-the-night-light-display-setting"></a>Aide sur le paramètre d’affichage en mode clair de nuit

Pour en savoir plus sur les paramètres d’affichage de nuit, consultez, [Définir l’affichage en mode nuit dans Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Si les options du mode clair de nuit sont grisées dans les Paramètres, vérifiez votre pilote d’affichage : 

1. Dans la zone de recherche de la barre des tâches, tapez **Gestionnaire d’appareil**, puis sélectionnez **Gestionnaire d’appareil** dans les résultats de la recherche.
1. Développez l’option **Afficher des adaptateurs**. 

Malheureusement, la fonctionnalité du mode clair de nuit n’est pas disponible, si votre appareil utilise un pilote DisplayLink ou un pilote Affichage simple.

La fonctionnalité du mode clair de nuit utilise la technologie graphique récente. La mise à jour de votre pilote d’affichage pourrait donc être nécessaire :  

- Recherchez les mises à jour en accédant à **Démarrer** > **Paramètres** > **Mise à jour et sécurité** > **Windows Update** > **Vérifier les mises à jour**.  

OU

- Visitez le site web du support de votre fabricant de matériel pour télécharger et installer manuellement les derniers pilotes d’affichage.

## <a name="reset-night-light-in-the-registry"></a>Réinitialiser le mode clair de nuit dans le registre

Si la mise à jour de votre pilote d’affichage n’a pas fonctionné, vous devrez peut-être réinitialiser le mode clair de nuit dans le registre.  

**Attention :** Cette étape de la résolution de problèmes est recommandée uniquement pour des utilisateurs avancés. Des problèmes graves peuvent se produire si vous modifiez le registre de façon incorrecte. Pour une protection supplémentaire, veuillez sauvegarder le registre avant de le modifier, afin de pouvoir le restaurer en cas de problème.

1. Dans la zone de recherche, tapez **Regedit**, puis sélectionnez **Éditeur de registre** dans les résultats de  recherche.

1. Accédez à cette clé de registre : 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exportez, puis supprimez cette valeur subkey:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exportez, puis supprimez cette valeur subkey:$$windows.data.bluelightreduction.settings

1. Redémarrez Windows et vérifiez si les options du mode clair de nuit sont disponibles.


