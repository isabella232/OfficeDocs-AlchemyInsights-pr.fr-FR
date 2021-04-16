---
title: Erreur Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786667"
---
# <a name="4c7-error-in-microsoft-teams"></a>Erreur 4c7 dans Microsoft Teams

Cette erreur se produit car Microsoft Teams requiert l'authentification par formulaires. Lorsque vous déployez les services AD FS (Active Directory Federation Services), l'authentification par formulaires n'est pas activée pour l'intranet par défaut. Si l'authentification intégrée Windows échoue, vous êtes invité à vous inscrire à l'aide de l'authentification par formulaires.

Pour résoudre ce problème, activez l'authentification par formulaires à l'aide du logiciel en snap-in MMC (Microsoft Management Console) AD FS sur l'ordinateur qui dispose de la copie locale d'Active Directory. Pour cela, procédez comme suit : 

1. Dans le volet de navigation, accédez aux stratégies **d'authentification.**
2. Sous **Actions dans** le volet d'informations, **sélectionnez Modifier l'authentification principale globale.**
3. Sous **l'onglet Intranet,** sélectionnez **Authentification par formulaires.**
4. Sélectionnez **OK** (ou **Appliquer).**