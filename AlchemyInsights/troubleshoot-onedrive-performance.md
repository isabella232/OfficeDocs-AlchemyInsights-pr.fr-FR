---
title: Résoudre les problèmes de performances de OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 22d5e2b24ac9bdd70b0bb0a9a6e1a0af29ef2c0f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533913"
---
# <a name="troubleshoot-onedrive-performance"></a>Résoudre les problèmes de performances de OneDrive

Si vous rencontrez une synchronisation plus lente que prévu ou des problèmes de performances similaires avec OneDrive:

- Vérifiez qu’il n’y a pas de problèmes connus à l’aide du [tableau de bord d’État du service](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fportal.office.com%2Fadminportal%2Fhome%23%2Fservicehealth&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051385661&sdata=z3OU7adaVjJorTGK8v7Ipo35E5vkk35lVCEzgGYQoNo%3D&reserved=0).

- [Activez les fichiers à la demande](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fsave-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051395670&sdata=QN1F4v1q6pNV2hIZ5LCZTtIbuv%2FR7lH5C5g%2FAFJQhrM%3D&reserved=0) afin de pouvoir accéder à tous vos fichiers dans OneDrive sans avoir à les télécharger tous et à utiliser l’espace de stockage sur votre appareil.

- [Passez en revue les meilleures pratiques](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Foffice365%2Fenterprise%2Fnetwork-planning-and-performance&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=RQCPPj7XPAm4IK6jKf1xugHnxXqqJoKK%2BlEENg7WrDQ%3D&reserved=0) pour la planification et les performances du réseau.

- Optimisez la vitesse de téléchargement [et de téléchargement](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FMaximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=vR4z9GSeObeKY3ouE7oru4Vr%2FGn%2FghUoFBjpRQbfvhA%3D&reserved=0), en particulier si vous synchronisez un appareil pour la première fois.

- Si vous synchronisez une bibliothèque avec plus de 100 000 éléments, la synchronisation OneDrive peut sembler bloquée longtemps ou l’état indique le traitement de la 0KB de xMB. " [En savoir plus sur la synchronisation de plus de 100 000 fichiers](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23synctoomany&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051415686&sdata=E4zeoBeRBnlGB1haZXTy%2FJfXMBWSPZCbp6JQvt5qX2o%3D&reserved=0) , ainsi que sur [la limite de 300 000 fichiers pris en charge par OneDrive](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23numberitemscanbesynced&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051425695&sdata=uqBKB3ykz9QDOPRmSf5YIKBUiNa57IdQVzeLZWL%2BMWc%3D&reserved=0).

- Lorsqu'un utilisateur dépasse les limites d'utilisation, SharePoint Online limitations des autres requêtes destinées à partir de ce compte d'utilisateur pour une courte période. Toutes les actions de l'utilisateur sont limitées alors que la limitation est en vigueur.
