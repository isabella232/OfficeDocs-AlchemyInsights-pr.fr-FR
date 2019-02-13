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
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918826"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Accès refusé lors de l’affichage d’un flux de travail

Flux de travail SharePoint 2013 qui tentent d’envoyer un message électronique à un groupe SharePoint peut échouer avec un message d’erreur « Accès refusé » si l’appartenance au groupe SharePoint n’est pas défini sur tout le monde.
  
 **Pour résoudre ce problème, procédez comme suit :**
  
 1. Autoriser tout le monde afficher les membres du groupe SharePoint. 
  
 2. Supprimer du groupe SharePoint dans les zones à ou CC ligne du courrier électronique. 
  
 3. Ajoutez explicitement les utilisateurs pour le champ à ou CC de ligne si la visibilité de l’appartenance ne peut pas être modifiée pour un groupe SharePoint. 
  
Pour afficher plus d’informations, consultez [HTTP non autorisés à /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

