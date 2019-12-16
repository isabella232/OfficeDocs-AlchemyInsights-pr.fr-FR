---
title: Accès refusé lors de l’affichage d’un flux de travail
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050523"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accès refusé lors de l’affichage d’un flux de travail

Les flux de travail SharePoint 2013 qui tentent d’envoyer un courrier électronique à un groupe SharePoint peuvent échouer avec un message d’erreur « Accès refusé » si l’appartenance au groupe SharePoint n’est pas définie sur tout le monde.
  
 **Pour résoudre ce problème, procédez comme suit :**
  
 1. Autoriser tout le monde à voir les membres du groupe SharePoint.
  
 2. Supprimez le groupe SharePoint de la ligne à ou CC du message électronique.
  
 3. Ajoutez explicitement les utilisateurs à la ligne à ou CC si la visibilité de l’appartenance ne peut pas être modifiée pour le groupe SharePoint.
  
Pour plus d’informations, reportez-vous à la rubrique [http Unauthorized to/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  