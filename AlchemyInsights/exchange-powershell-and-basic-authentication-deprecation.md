---
title: Exchange PowerShell et la dépréciation de l’authentification de base
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
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069242"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell et la dépréciation de l’authentification de base

Pour obtenir les informations les plus récentes sur la connexion à Exchange Online PowerShell sans utiliser l’authentification de base, [veuillez cliquer ici](https://aka.ms/exops-docs). Le module PowerShell V2 n’utilise pas l’authentification de base.

Veuillez noter que l’authentification de base doit rester activée sur l’ordinateur de votre client.
Le nouveau module PowerShell V2 utilise l’authentification moderne pour établir la connexion permettant d’activer toutes les applets de commande V2 se basant sur REST. Outre les applets de commande V2, elle vous permet également d’accéder à applets de commande Remote PowerShell (RPS) plus anciennes nécessitant l’établissement d’une session PowerShell à distance. L’établissement d’une session RPS sur un ordinateur Windows nécessite l’activation de WinRM BasicAuth sur l’ordinateur client, même si le module utilise un mécanisme d’authentification moderne pour s’authentifier auprès du service. Le pipeline WinRM BasicAuth est utilisé pour transporter des jetons d’authentification modernes. Si WinRM BasicAuth est désactivée sur l’ordinateur client, les nouvelles applets de commande V2 continueront de fonctionner (à la différence des applets de commande RPS plus anciennes).
