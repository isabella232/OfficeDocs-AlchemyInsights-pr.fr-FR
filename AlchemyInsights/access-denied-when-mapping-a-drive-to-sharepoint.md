---
title: Accès refusé lors du mappage d’un lecteur SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 1ed67ec926c3e73f7a16b927729255505dfe93a0ae442a5dff9400afafb41d8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938729"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Résoudre les problèmes liés SharePoint bibliothèques mappées sur des lecteurs réseau

Lorsque vous accédez à un lecteur réseau mappé, vous pouvez voir l’un des messages suivants :
  
- **\\Le chemin d’accès n’est pas accessible. Vous n’êtes peut-être pas autorisé à utiliser cette ressource réseau. Contactez l’administrateur de ce serveur pour savoir si vous avez des autorisations d’accès.**

- **Accès refusé. Avant d’ouvrir des fichiers à cet emplacement, vous devez d’abord ajouter le site web à votre liste des sites de confiance, accéder au site web et sélectionner l’option de connexion automatique.**

[Obtenez de l’aide pour résoudre les problèmes de lecteurs réseau mappés.](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)
  
Le mappage d’une bibliothèque en tant que lecteur réseau est temporaire et pris en charge uniquement dans Internet Explorer. Au lieu de cela, [synchronisez SharePoint fichiers avec](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) le nouveau client Synchronisation OneDrive qui inclut [fichiers à la demande](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Accédez à l’ensemble de vos fichiers dans OneDrive sans utiliser l’espace de stockage local.
  