---
title: Créer et utiliser une boîte aux lettres partagée
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717345"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Résoudre le problème-utilisateur introuvable dans l’annuaire

<p>Si les utilisateurs reçoivent un message <strong> &ldquo; &hellip;d’erreur&rsquo;, l’utilisateur peut se trouver dans l’annuaire. Veuillez réessayer&hellip; </strong> là où le type de problème est l' <strong> &ldquo;utilisateur qui&rdquo;n’est pas dans le répertoire.</strong>, les étapes suivantes peuvent être effectuées pour résoudre le problème.</p> <ol> <li>Assurez-vous que le compte qui a accepté l’invitation électronique est le même compte que celui utilisé pour la connexion ultérieure. Assurez-vous que l’utilisateur utilise le même compte pour accepter l’invitation et se connecter au site. <br /><br />Pour plus d’informations, reportez-vous à la rubrique <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">gestion des alias de votre compte Microsoft</a> pour gérer la connexion à Office 365. <br /><br /></li> <li>Accédez à chaque site (s) dans lequel l’utilisateur reçoit l’erreur. <br /><br />a. Ajoutez <strong> &ldquo;/_layouts/15/People.aspx/MembershipGroupId = 0&rdquo; </strong> (dans les guillemets doubles) à la fin de l’URL du site. <br /><br />Exemple: https://&lt;contoso&gt;. SharePoint.com/_layouts/15/People.aspx/membershipGroupId=0 <br /><br />b. Sélectionnez l’utilisateur dans la liste. <br /><br />c. Cliquez sur <strong>Supprimer les autorisations des utilisateurs du ruban</strong>. <br /><br />d. Rajoutez l’utilisateur et renvoyez-le à l’utilisateur.</li> </ol>

