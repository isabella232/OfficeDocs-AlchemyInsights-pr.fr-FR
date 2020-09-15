---
title: Résoudre les problèmes de chargement d’images dans Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690241"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Résoudre les problèmes de chargement d’images dans Yammer

Lorsque des problèmes liés aux photos et aperçus de fichiers sont détectés dans Yammer, résolvez les problèmes en vérifiant si le problème se produit pour tous les utilisateurs, s'il se produit sur les appareils mobiles et s'il est reproductible lors du chargement de la pièce jointe.  

**Problèmes de photo de profil**  

Si les utilisateurs finaux se connectent à Yammer via Microsoft 365, ils doivent modifier leur profil, y compris leur photo de profil. Si les utilisateurs ne sont pas autorisés à effectuer des mises à jour de profil, un administrateur peut effectuer la mise à jour pour l’utilisateur. Pour plus d’informations, voir [Afficher et mettre à jour votre profil dans Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Pour plus d’informations sur la modification de profil, notamment les photos de profil, consultez [Modifier mon profil et paramètres Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Les photos de profil mises à jour sont synchronisées différemment par rapport aux attributs de profil. Les utilisateurs doivent se connecter pour lancer la synchronisation de leur photo de profil. Pour plus d’informations, consultez la rubrique [Les images de profil utilisateur mises à jour dans Office 365 le sont-elles également dans Yammer ?](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Pour plus d’informations sur le cycle de vie des utilisateurs de Yammer, consultez l’article [Gérer les utilisateurs de Yammer tout au long de leur cycle de vie à partir d’Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Pour plus d’informations sur le fonctionnement de la synchronisation de la photo de profil dans Microsoft 365, consultez l’article [Informations sur la synchronisation de la photo de profil dans Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Aperçus de documents et problèmes de miniatures**  

Lors de la publication de fichiers ou d’images dans Yammer, des aperçus peuvent ne pas s’afficher pour les raisons suivantes : 

- Le fichier est endommagé et ne peut pas être traité.
- Le fichier n'a pas été récemment chargé sur SharePoint Online, ou Yammer contient des métadonnées non valides pour d'autres raisons.
- Les URL nécessaires au chargement des images d'aperçu sont bloquées.
- L’aperçu du fichier a été supprimé par l’utilisateur avant la publication.
- Un problème de service a empêché la génération d’aperçus.

**Remarque** les aperçus des liens et des chargements de fichiers peuvent se comporter différemment. Il se peut que des liens vers des fichiers sur Internet ou des liens nécessitant une authentification supplémentaire ne s’affichent pas correctement.

Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Joindre un fichier ou une image à un message de Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 