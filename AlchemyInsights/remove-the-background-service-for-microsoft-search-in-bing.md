---
title: Supprimer le service d’arrière-plan pour la Recherche Microsoft dans Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753414"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Supprimer le service d’arrière-plan pour la Recherche Microsoft dans Bing

Pour supprimer le service d’arrière-plan pour Recherche Microsoft dans Bing, vous pouvez essayer ce qui suit :

1. Pour revenir aux paramètres du moteur de recherche d’origine, vous pouvez effectuer les opérations suivantes :

    a. Commutez le **[bouton bascule](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Utiliser Bing comme moteur de recherche par défaut sur Désactivé**.

    b. [Accédez au Centre d’administration Microsoft 365,](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) et effacez le paramètre qui affecte tous les utilisateurs de votre organisation.

2. Pour supprimer le service d’arrière-plan d’un appareil individuel, effectuer les tâches suivantes :

    a. Sélectionnez **Panneau de configuration > Programmes > Programmes et fonctionnalités**.

    b. Cliquez avec le bouton **Recherche Microsoft dans Bing** sous la liste des programmes installés, puis cliquez sur **Désinstaller**.

3. Pour supprimer le service d’arrière-plan de plusieurs appareils dans votre organisation, connectez-vous en tant qu’administrateur et exécutez la commande suivante dans un script : 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
