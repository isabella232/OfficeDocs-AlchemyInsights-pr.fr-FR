---
title: Erreur 4C7 teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796104"
---
# <a name="4c7-error-in-microsoft-teams"></a>erreur 4C7 dans Microsoft teams

Cette erreur se produit parce que Microsoft teams nécessite l’authentification par formulaire. Lorsque vous déployez Active Directory Federation Services (AD FS), l’authentification par formulaire n’est pas activée par défaut pour l’intranet. Si l’authentification Windows intégrée échoue, vous êtes invité à vous connecter à l’aide de l’authentification par formulaire.

Pour résoudre ce problème, activez l’authentification par formulaire à l’aide du composant logiciel enfichable MMC (Microsoft Management Console) AD FS sur l’ordinateur disposant de la copie locale d’Active Directory. Pour cela, procédez comme suit: 

1. Dans le volet de navigation, accédez à **stratégies d’authentification**.
2. Sous **actions** dans le volet d’informations, sélectionnez **modifier l’authentification principale globale**.
3. Sous l’onglet **Intranet** , sélectionnez **authentification par formulaire**.
4. Sélectionnez **OK** (ou **appliquer**).