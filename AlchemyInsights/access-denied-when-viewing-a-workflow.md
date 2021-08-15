---
title: Accès refusé lors de l’affichage d’un flux de travail
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955199"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accès refusé lors de l’affichage d’un flux de travail

SharePoint 2013 Les flux de travail qui tentent d’envoyer un courrier électronique à un groupe SharePoint peuvent échouer avec un message d’erreur « Accès refusé » si l’appartenance au groupe SharePoint n’est pas définie sur Tout le monde.
  
 **Pour résoudre ce problème, faites les étapes suivantes :**
  
 1. Autorisez tout le monde à voir les membres du SharePoint groupe.
  
 2. Supprimez le SharePoint de la ligne À ou Cc de l’e-mail.
  
 3. Ajoutez explicitement les utilisateurs à la ligne À ou Cc si la visibilité de l’appartenance ne peut pas être modifiée pour SharePoint groupe.
  
Pour plus d’informations, reportez-vous à [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  