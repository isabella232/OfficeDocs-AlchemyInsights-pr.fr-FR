---
title: Utiliser TeamViewer pour gérer à distance les appareils Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 35c82f8b91a4a0a75f8aa376771a20e6684620c55e8a06abe59db22cab945139
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53990525"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Utiliser TeamViewer pour gérer à distance les appareils Intune

Les appareils gérés par Intune peuvent être administrés à distance à l’aide de [TeamViewer](https://www.teamviewer.com/).

Pour gérer Intune à l’aide de TeamViewer, procédez comme suit : 

Commencez par obtenir les informations d’identification de TeamViewer pour configurer le connecteur TeamViewer sur Intune. Cela permet à l’administrateur d’entrer des informations d’identification dans l’interface utilisateur du connecteur TeamViewer sous Appareils, une opération ponctuelle pour établir le lien entre Intune et le service TeamViewer.

**Partie 1 : démarrer une session avec un appareil distant**

1. Sous **Tous les appareils**, sélectionnez l’appareil avec lequel vous voulez démarrer une session à distance.
2. À partir de **... Plus**, sélectionnez **Nouvelle session d’assistance à distance**.
3. Sélectionnez **Oui** pour confirmer que vous voulez établir une session à distance.
    Une fois que la demande « Lancer une nouvelle session à distance » est reconnue par le service TeamViewer, une option vous permettant de **Démarrer l’assistance à distance** s’affiche sous les détails du volet Vue d’ensemble (ou, Essentiels) pour l’appareil. Sélectionnez **Afficher plus** pour développer le volet et afficher l’état de l’assistance à distance.
4. Sélectionnez **Démarrer une session à distance** pour démarrer la session côté administrateur.
5. Choisissez de télécharger le fichier binaire TeamViewer (Windows), puis sélectionnez **Exécuter**.<br/>
    **Remarque** vous pouvez ignorer toute page de navigateur web ouverte sur le site web TeamViewer.

6. Accusez réception de la demande d’application TeamViewer pour apporter des modifications sur l’appareil (Windows uniquement).
7. L’application TeamViewer démarre et inclut le code de session authentifiant la connexion avec l’appareil distant.

**Partie 2 : sur l’appareil ciblé pour une session à distance**

1. Ouvrez le Portail d’entreprise Intune.
2. Recherchez un indicateur de notification : « Votre administrateur informatique demande le contrôle de cet appareil pour une session d’assistance à distance », puis sélectionnez la notification.
3. Choisissez de télécharger l’application TeamViewer, ou d’accuser réception du téléchargement de l’application TeamViewer à partir de l’App Store, puis sélectionnez **Exécuter**.
    **Remarque** vous pouvez ignorer toute page de navigateur web ouverte sur le site web TeamViewer.

4. Accusez réception de la demande d’application TeamViewer pour apporter des modifications sur l’appareil (Windows uniquement).
5. L’application TeamViewer démarre et inclut le code de session authentifiant la connexion avec l’appareil distant.
6. Une fenêtre contextuelle vous demande si vous voulez autoriser le démarrage de la session.

**Remarque** les codes de session générés par le service TeamViewer sont à usage unique. Si vous perdez la connexion, vous devez :

1. Fermer l’instance de l’application TeamViewer sur l’appareil distant et sur la station de travail d’administration.
2. Fermer le Portail de l’entreprise sur l’appareil distant.
3. Lancer une nouvelle session d’assistance à distance à partir du Portail d’administration.
4. Rouvrir le portail de l’entreprise sur l’appareil distant pour recevoir la nouvelle notification.
5. Télécharger et ouvrir l’application TeamViewer sur l’appareil distant et la station de travail d’administration, comme précédemment.