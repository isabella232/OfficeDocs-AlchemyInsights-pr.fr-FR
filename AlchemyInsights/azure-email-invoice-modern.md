---
title: Envoi de la facturation par e-mail dans Azure moderne
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
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082832"
---
# <a name="email-invoicing-in-azure"></a>Envoi de la facturation par e-mail dans Azure

Vous devez posséder le rôle de propriétaire ou de collaborateur sur le profil de facturation ou son compte de facturation pour mettre à jour ses préférences de facturation par e-mail. Après activation, tous les utilisateurs disposant de rôles de propriétaire, de contributeur, de lecteur et de gestionnaire de factures dans un profil de facturation reçoivent la facture correspondante par e-mail.

1. Connectez-vous au [portail Azure](https://portal.azure.com/).
2. Recherchez **Gestion des coûts + Facturation**.
3. Sélectionnez **Factures** dans le côté gauche, puis **Facture par e-mail** en haut de la page.
4. Si vous possédez plusieurs profils de facturation, sélectionnez-en un, puis choisissez **Activation**.

5. Sélectionnez **Mettre à jour**.
6. Si vous possédez plusieurs profils de facturation, sélectionnez-en un, puis choisissez **Activation**.

Vous autorisez d’autres personnes à afficher, télécharger et régler les factures en leur attribuant le rôle de gestionnaire de factures pour un profil de facturation MCA ou MPA. Si vous avez activé l’envoi des factures par e-mail, les utilisateurs reçoivent également les factures par e-mail.

1. Connectez-vous au [portail Azure](https://portal.azure.com/).
2. Recherchez **Gestion des coûts + Facturation**.
3. Sélectionnez **Profils de facturation** dans le côté gauche. Dans la liste des profils de facturation, sélectionnez celui auquel vous voulez attribuer un rôle de gestionnaire de factures.
4. Sélectionnez **Contrôle d’accès (IAM)** dans le côté gauche, puis **Ajouter** en haut de la page.

Dans la liste déroulante Rôle, sélectionnez **Gestionnaire de factures**. Entrez l’adresse e-mail de l’utilisateur pour lui donner accès. Sélectionnez **Enregistrer** pour attribuer le rôle.
