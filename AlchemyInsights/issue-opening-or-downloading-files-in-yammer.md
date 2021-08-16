---
title: Problème d’ouverture ou de téléchargement de fichiers dans Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028254"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problème d’ouverture ou de téléchargement de fichiers dans Yammer

La version classique de Yammer prend en charge plusieurs options de chargement de fichiers dans les messages et les groupes. Selon la configuration du réseau, les fichiers sont stockés par défaut dans SharePoint.

Le sélecteur de fichiers dans la nouvelle version de Yammer ne prend pas encore en charge toutes les options disponibles dans la version classique de Yammer. Une prochaine mise à jour permet d’ajouter des fonctionnalités supplémentaires. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Joindre un fichier ou une image à un billet de conversation Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Impossible d’ouvrir ou de télécharger un fichier**  

Vous pouvez charger un fichier sur Yammer, mais aussi le relier à un fichier dans SharePoint Online. Pour résoudre ce problème, vous devez tout d’abord déterminer l’emplacement du fichier. Si vous avez chargé le fichier sur Yammer, vous verrez que l’URL comporte *.yammer.com. Assurez-vous que les URL et adresses IP requises sont débloquées. Si vous souhaitez en savoir plus, veuillez consulter le billet de blog [L’utilisation d’adresses IP codées en dur pour Yammer n’est pas recommandée](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Vérifiez si un utilisateur qui est également un administrateur général peut télécharger le fichier. Si le fichier est privé, vous devrez peut-être utiliser le mode Contenu privé. Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Surveiller le contenu privé dans Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Invités et fichiers au niveau du réseau Yammer dans SharePoint Online**  

[Les invités au niveau du réseau dans Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) n’utilisent pas Azure AD B2B et sont internes au service Yammer, de sorte qu’ils ne peuvent pas accéder aux fichiers Yammer stockés dans SharePoint. Créez un utilisateur AAD B2B externe pouvant accéder aux bibliothèques de documents dans SharePoint Online à l’aide de cette identité. Si vous souhaitez en savoir plus sur la prochaine prise en charge de l’invité Azure AD B2B dans Yammer, veuillez consulter la rubrique [Prise en charge de l’invité Business-to-Business (B2B) dans la version préliminaire de Yammer –Conditions client et FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).