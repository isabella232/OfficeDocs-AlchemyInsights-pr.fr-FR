---
title: 'État du domaine : aucun service sélectionné'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389179"
---
# <a name="domain-status---no-services-selected"></a>État du domaine : aucun service sélectionné

**Aucun service** sélectionné signifie que vous n’avez pas sélectionné de services Microsoft 365 tels que Exchange Online, Skype Entreprise ou Intune, et gestion des périphériques mobiles pour Microsoft 365 à utiliser avec votre domaine personnalisé. Si vous utilisez un filtrage hybride Exchange (Exchange local avec Exchange Online) ou un filtrage de courrier indésirable externe avec Exchange et aucune autre services Microsoft, vous pouvez ignorer ce message. L’état d’état du domaine est disponible uniquement pour les domaines connectés directement au service.

Pour sélectionner des services pour votre domaine :

1. À   >  [**Paramètres, cochez**](https://admin.microsoft.com/Adminportal/Home)la case en regard du domaine avec le message d’état Aucun **service sélectionné.**
1. Sélectionnez **Gérer le DNS** pour démarrer l’Assistant Configuration de domaine.
    - Si vous choisissez **Ajouter vos propres enregistrements DNS,** n’oubliez pas de sélectionner un service lorsque vous y êtes invité. D’autres services peuvent être disponibles sous **Options avancées.**
    - Si vous choisissez Laisser Microsoft ajouter vos enregistrements **DNS** ou d’autres **options** Configurer mes services en ligne pour moi, tous les services disponibles sont suggérés et sélectionnés  >   automatiquement.
1. Continuez à l’aide de l’Assistant pour terminer la configuration DNS et vos choix de service.
 
Pour obtenir de l’aide supplémentaire sur la configuration de votre domaine, voir Ajouter des enregistrements [DNS pour connecter votre domaine.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

