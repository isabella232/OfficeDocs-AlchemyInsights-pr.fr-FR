---
title: Accès refusé lors de l’affichage d’un flux de travail
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883589"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accès refusé lors de l’affichage d’un flux de travail

Les flux de travail SharePoint 2013 qui tentent d’envoyer un courrier électronique à un groupe SharePoint peuvent échouer avec un message d’erreur «Accès refusé» si l’appartenance au groupe SharePoint n’est pas définie sur tout le monde.
  
 **Pour résoudre ce problème, procédez comme suit:**
  
 1. Autoriser tout le monde à voir les membres du groupe SharePoint.
  
 2. Supprimez le groupe SharePoint de la ligne à ou CC du message électronique.
  
 3. Ajoutez explicitement les utilisateurs à la ligne à ou CC si la visibilité de l’appartenance ne peut pas être modifiée pour le groupe SharePoint.
  
Pour plus d’informations, reportez-vous à la rubrique [http Unauthorized to/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  