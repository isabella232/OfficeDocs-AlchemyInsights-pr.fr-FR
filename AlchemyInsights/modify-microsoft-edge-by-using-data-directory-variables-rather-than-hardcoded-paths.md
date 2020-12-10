---
title: Modifier Microsoft Edge à l’aide de variables de répertoire de données plutôt que de chemins d’accès codés
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608843"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="d1339-102">Modifier Microsoft Edge à l’aide de variables de répertoire de données plutôt que de chemins d’accès codés</span><span class="sxs-lookup"><span data-stu-id="d1339-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="d1339-103">Par exemple, sous Windows, pour stocker les données de profil sous les données d’application locale d’un utilisateur plutôt que dans l’emplacement par défaut, définissez la stratégie **UserDataDir** sur **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="d1339-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="d1339-104">Pour plus d’informations, consultez la rubrique [Create Microsoft Edge User Data Directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span><span class="sxs-lookup"><span data-stu-id="d1339-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>