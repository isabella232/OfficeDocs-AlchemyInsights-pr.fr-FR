---
title: Notifications dans Yammer
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
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833577"
---
# <a name="notifications-in-yammer"></a>Notifications dans Yammer

Pour vous signaler une nouvelle activité dans le cadre de conversations pertinentes, [Yammer envoie des notifications](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) par courrier électronique ou, si vous utilisez Yammer sur votre appareil mobile, via les notifications push. Par défaut, Yammer vous envoie des notifications pour de nombreux types d’activités sur votre réseau. Les utilisateurs peuvent mettre à jour leur paramètres de courrier via le site web Yammer, et les notifications push sont configurées via l’application mobile. 

Yammer a ajouté la prise en charge des [messages électroniques interactifs dans Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Certains messages électroniques (copie de message) deviennent interactifs dans Outlook sur le web. Une prochaine mise à jour permet d’accéder à d’autres versions d’Outlook.

**Types de notifications dans Yammer**

- Les messages électroniques (mises à jour d’un groupe, une personne vous invite à un groupe, vous recevez un message dans votre boîte de réception, etc.).
- Notifications push (envoyées aux appareils mobiles lorsque vous y êtes mentionné, recevoir un message dans votre boîte de réception, etc.)
- Fenêtres contextuelles de bureau (lorsque l’application de bureau Yammer est installée, elle affiche les notifications pour les utilisateurs appelés notifications « Toast »).
- Notifications cloche (à l’intérieur du site web Yammer), les utilisateurs verront des notifications pour différents événements. Il est possible que ces notifications n’aient pas toujours de message de notification ou de transmission associé.)

D’autres [informations plus détaillées sur les notifications](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) sont disponibles.

**Gestion des notifications**

Les utilisateurs doivent gérer leurs propres notifications. Les informations sont disponibles dans l’article [l’activation et la désactivation des notifications par courrier électronique et mobiles Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Il n’est pas possible pour les administrateurs de désactiver toutes les notifications, ou de contrôler les notifications, au nom des utilisateurs. Les administrateurs peuvent [contrôler le logo inclus dans les messages électroniques, et si les utilisateurs doivent confirmer les messages](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) publiés par courrier électronique.

**Notifications envoyées par courrier électronique à de nombreux utilisateurs au sein de votre organisation**

Il peut arriver qu’une notification par courrier électronique soit envoyée par Yammer et reçue par de nombreux utilisateurs au sein de votre organisation. Cela se produit lorsqu’une liste de distribution, ou un autre type d’adresse de courrier non individuelle, est ajoutée à Yammer. Yammer ne sait pas, dans tous les cas, si une adresse de courrier appartient à un seul utilisateur ou s’il s’agit d’une adresse de messagerie qui entraîne la remise d’un message électronique à plusieurs destinataires. Lorsque ce problème se produit, vous devez prendre des mesures pour [suspendre (désactiver) l’utilisateur non valide avec cette adresse de courrier](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) dans Yammer. 

Pour réduire le risque que ce problème se produise, procédez comme suit :

1. [Appliquer l'identité Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) pour Yammer.
2. Empêcher les expéditeurs externes d’envoyer des courriers électroniques à votre organisation, ou limiter les expéditeurs à une liste approuvée.

Si ce problème se produit :

1. Identifiez le destinataire du message électronique, qui doit correspondre à l’utilisateur dans Yammer. Par exemple, all-in-sales@fabrikam.com est une DL pour tous les commerciaux. Cette DL peut être identifié à partir de la messagerie Yammer reçue par les utilisateurs.
2. Utilisez la fonctionnalité de [désactiver (suspendre) dans Administration du réseau](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) pour suspendre l’utilisateur possédant l’adresse de courrier all-in-sales@fabrikam.com. La suspension peut être annulée. par conséquent, il est plus sûr que la suppression. La suppression de l’utilisateur aura lieu automatiquement après 90 jours.
3. Vous pouvez également passer en revue [Exportation d'un utilisateur](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) pour identifier les autres adresses de messagerie non-utilisateur qui doivent être suspendues.
