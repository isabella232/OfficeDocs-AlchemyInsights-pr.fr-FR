---
title: 'Thème de Teams : fourre-tout'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2605"
- "9000701"
ms.openlocfilehash: 47e9aa76f8624ce3ddf4cfd03637b5b2714eb435
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030398"
---
# <a name="teams-common-issues-and-resolutions"></a>Problèmes courants de Teams et résolutions

**Important** : en raison d’une hausse récente de l’utilisation de Teams, lorsque vous attribuez une licence Teams à un utilisateur, sa configuration complète peut prendre environ 24 heures. En attendant, vous ne serez pas en mesure d’affecter des stratégies Teams à celui-ci, et il ne pourra peut-être pas accéder à certaines fonctionnalités de Teams telles que l’appel et l’audioconférence.

**Problèmes courants et leur résolution**

Pour obtenir une réponse plus précise, essayez de reformuler votre question afin d’y inclure toutes les erreurs rencontrées ou les fonctions de Teams utilisée.

Si vous avez besoin d’aide pour déployer Teams afin de prendre en charge les travailleurs à distance (WFH) en raison du COVID-19, consultez la section [Prise en charge des travailleurs à distance avec Microsoft Teams](https://docs.microsoft.com/microsoftteams/support-remote-work-with-teams). De plus, vous aurez sans doute droit à une aide au déploiement dans le cadre du programme Microsoft 365 FastTrack. Visitez le [centre FastTrack](https://www.microsoft.com/fasttrack) pour envoyer une demande.

Pour tous les clients Teams :

- **Vous débutez avec Teams ?** Voir [Prise en main de Microsoft Teams](https://docs.microsoft.com/microsoftteams/get-started-with-teams-quick-start).
- **Autoriser l’accès invité Teams :** examinez la [liste de contrôle d’accès invité Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) et vérifier que toutes les étapes ont été effectuées. Ressources supplémentaires :
    - [Comprendre l'accès invité dans Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Configuration : Liste de contrôle d'accès invité Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Comment un invité rejoint une Équipe](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Réunions et rendez-vous Teams** : Avez-vous besoin d’aide pour activer ou configurer l’audioconférence dans Microsoft Teams ? Cet utilisateur a-t-il été créé récemment ? Si c’est le cas, vous devez attendre 2 à 24 h **pour que les paramètres prennent effet**. 

    Pour vérifier que l’utilisateur dispose d’une licence pour l’audioconférence et possède un numéro payant par défaut :
    1.    Accédez à utilisateurs actifs, puis sélectionnez l’utilisateur concerné.
    2.    Selon la version du centre d’administration, choisissez **Licences et applications** ou cliquez sur **Modifier** dans **Licences de produits**.
    3.    Vérifiez que l’utilisateur a sélectionné des licences pour l’Audioconférence, Microsoft Teams et Skype Entreprise Online (plan 2).
    4.    Les centres d'administration des utilisateurs cliquent sur **Afficher tout**, puis sur **Teams**.
    5.    Dans le centre d’administration Microsoft Teams, cliquez sur **Portail hérité**.
    6.    Dans le centre d’administration Skype Entreprise, cliquez sur **Audioconférence**, puis sur **Utilisateurs**.
    7.    Sélectionnez l’utilisateur concerné et vérifiez que celui-ci dispose d’un numéro payant par défaut.
    
    Pour plus d’informations, voir [Plans d’appels pour Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) ou appelez l’équipe de facturation Microsoft Commerce pour obtenir de l’aide sur les questions liées à la gestion des licences.

    Ressources supplémentaires :

    - [Réunions et conférences dans Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audioconférence dans Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Licences exploratoires pour les équipes**: l’expérience exploratoire de Microsoft Teams permet aux utilisateurs de votre organisation qui ont Azure Active Directory (AAD) et qui ne disposent pas d’une licence pour les équipes de lancer une expérience exploratoire des équipes. Les administrateurs peuvent activer ou désactiver cette fonctionnalité pour les utilisateurs de leur organisation. La précédente [Version d'évaluation dans le cloud commercial Microsoft](https://docs.microsoft.com/microsoftteams/iw-trial-teams) est désormais remplacée par l'expérience exploratoire Teams.

    Ressources supplémentaires :

    - [Comment les utilisateurs s’inscrivent pour l’expérience exploratoire Teams ?](https://docs.microsoft.com/microsoftteams/teams-exploratory#how-users-sign-up-for-the-teams-exploratory-experience)
    - [Gérer l’expérience d’exploration de Teams](https://docs.microsoft.com/microsoftteams/teams-exploratory#manage-the-teams-exploratory-experience)

- **Canaux privés**: les canaux privés dans Microsoft Teams créent des espaces ciblés pour la collaboration au sein de vos équipes. Seuls les utilisateurs de l’équipe qui sont propriétaires ou membres du canal privé peuvent accéder au canal. Tous les utilisateurs, notamment les invités, peuvent être ajoutés en tant que membre d’un canal privé, dès lors qu’ils sont déjà membres de l’équipe.

    Vous souhaiterez peut-être utiliser un canal privé si vous souhaitez limiter la collaboration à ceux qui en ont besoin ou si vous souhaitez faciliter la communication entre un groupe de personnes affectées à un projet spécifique, sans avoir à créer une équipe supplémentaire à gérer.

    Ressources supplémentaires :
    - [Création et adhésion au canal privé](https://docs.microsoft.com/microsoftteams/private-channels#private-channel-creation-and-membership)
    - [Gérer les paramètres et l’appartenance au canal privé](https://docs.microsoft.com/microsoftteams/private-channels#manage-private-channel-membership-and-settings)

- **Stratégies de réunion**: les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles aux participants à la réunion pour les réunions planifiées par les utilisateurs au sein de votre organisation. Après avoir créé une stratégie et apporté vos modifications, puis vous pouvez affecter des utilisateurs à la stratégie. 
    - **Modifier ou créer une stratégie de réunion** : pour modifier ou créer une stratégie de réunion, accédez au **Centre d’administration Microsoft Teams > Réunions > Stratégies de réunion**. Sélectionnez une stratégie dans la liste ou cliquez sur Ajouter. Si vous créez une stratégie, ajoutez un nom et une description. Le nom ne peut pas contenir de caractères spéciaux et ne doit pas dépasser 64 caractères. Choisissez les paramètres, puis cliquez sur **Enregistrer**.

        Par exemple, imaginons que vous avez un grand nombre d’utilisateurs et que vous voulez limiter la quantité de bande passante requise par la réunion. Vous devez créer une stratégie personnalisée nommée « bande passante limitée » et désactiver les paramètres suivants :

        Sous ** Audio & vidéo** :
        - Désactivez l’option Autoriser l’enregistrement Cloud.
        - Désactivez Autoriser la vidéo IP.

        Sous **Partage de contenu** :
        - Désactiver le mode de partage d’écran.
        - Désactivez  Autoriser le tableau blanc.
        - Désactivez Autoriser les notes partagées.

        Vous pouvez ensuite attribuer la stratégie aux utilisateurs.

- **Affecter une stratégie de réunion aux utilisateurs**

    1. Dans le volet de navigation gauche du centre d’administration Microsoft Teams, et accédez aux **Utilisateurs**, puis cliquez sur l’utilisateur.
    2. Sélectionnez l’utilisateur en cliquant à gauche du nom de celui-ci, puis cliquez sur **Modifier les paramètres**.
    3. Sous **Stratégie de réunion**, sélectionnez la stratégie que vous souhaitez attribuer, et puis cliquez sur **Appliquer**.

    Pour attribuer une stratégie à plusieurs utilisateurs à la fois, consultez l’article [Modifier en masse les paramètres utilisateur Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk). Vous pouvez effectuer les opérations suivantes :

    1. Dans le volet de navigation gauche du centre d’administration Microsoft Teams, accédez aux **Réunions > Stratégies de réunion**.
    2. Sélectionnez la stratégie en cliquant à gauche du nom de celle-ci.
    3. Sélectionnez **Gérer les utilisateurs**.
    4. Dans le volet **Gérer les utilisateurs**, recherchez l’utilisateur par son nom complet ou son nom d’utilisateur, sélectionnez le nom, puis cliquez sur **Ajouter**. Répétez cette étape pour chaque utilisateur que vous souhaitez ajouter.
    5. Lorsque vous avez terminé d'ajouter les utilisateurs, cliquez sur **Enregistrer**.

- **Résoudre les problèmes liés à un pavé de numérotation manquant :**  

    - Vérifiez qu’une [licence Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) a été attribuée à l’utilisateur.
    - Vérifiez qu’un [plan d’appel](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) a été attribué à l’utilisateur.
    - Activer les utilisateurs pour [Voix Entreprise](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Résoudre les problèmes de connexion de Teams :** tout d’abord, vérifiez que le [service Microsoft Teams est sain](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Recherchez ensuite les codes d’erreur courants et révisez [Pourquoi est-ce que je rencontre des problèmes pour me connecter à Microsoft teams ?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)  Vous devrez sans doute revoir également [Modèles d’identité et authentification dans Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).

**Pour les clients Éducation :**

Si vos utilisateurs voient le message « vous allez rater quelque chose ! » Veillez à [activer Microsoft Teams pour votre école](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Dans les clients EDU, Microsoft Teams n’est pas activé par défaut ; vous devrez l’activer au préalable.

Ensuite, reportez-vous à la section [Enseignement à distance et formations dans Office 365 Éducation](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) pour découvrir les derniers conseils sur la configuration de votre établissement scolaire, la planification des leçons, les réunions virtuelles et le partage de contenu avec des étudiants.

Enfin, n’hésitez pas à consulter les vidéos de formation pour les administrateurs informatiques Microsoft Teams, les decks et bien plus encore :  https://docs.microsoft.com/MicrosoftTeams/itadmin-readiness#technical-training. 
