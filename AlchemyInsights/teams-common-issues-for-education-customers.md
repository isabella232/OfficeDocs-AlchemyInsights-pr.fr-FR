---
title: Problèmes courants de Teams pour les clients du secteur de l’éducation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 023bb40e54a1f1a87f0b618d49a812fc9dfda971
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737015"
---
# <a name="teams-common-issues-for-education-customers"></a>Problèmes courants de Teams pour les clients du secteur de l’éducation

**Pour les clients du secteur de l’éducation** :

Si vous avez besoin d’aide pour déployer Teams afin de prendre en charge la formation à distance, visitez le [Centre FastTrack](https://www.microsoft.com/fasttrack) pour envoyer une demande. Consultez les problèmes courants suivants de Teams pour les clients du secteur de l’éducation :

- Le message « **Vous allez rater quelque chose !**  » s’affiche Veillez à [activer Microsoft Teams pour votre école](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Dans les clients EDU, Microsoft Teams n’est pas activé par défaut ; vous devrez l’activer au préalable.

- **Vous débutez avec Teams ?** Consultez l’article [Enseignement et formation à distance dans Office 365 Éducation](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) pour découvrir les conseils les plus récents sur la configuration de votre établissement scolaire, la planification des cours, les réunions virtuelles et le partage de contenu avec les étudiants.

- Une fois activé, les utilisateurs peuvent exécuter Teams en installant la version [bureau](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) et les [clients mobiles](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) ou depuis le navigateur surhttps://teams.microsoft.com.

- **Activer l’accès invité Teams** : consultez la [liste de contrôle d’accès invité Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) et vérifier que toutes les étapes ont été effectuées.
    - [Comprendre l'accès invité dans Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Configuration : Liste de contrôle d'accès invité Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Comment un invité rejoint une Équipe](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Réunions et rendez-vous Teams** : Avez-vous besoin d’aide pour activer ou configurer l’audioconférence dans Microsoft Teams ? Cet utilisateur a-t-il été créé récemment ? Si c’est le cas, vous devrez attendre 2 à 24 heures pour que les paramètres prennent effet. Pour vérifier que l’utilisateur dispose d’une licence pour l’audioconférence et possède un numéro payant par défaut :
    1. Accédez aux Utilisateurs actifs, puis sélectionnez l’utilisateur concerné.
    2. Selon la version du centre d’administration, choisissez **Licences et applications** ou cliquez sur **Modifier** dans **Licences de produits**.
    3. Vérifiez que l’utilisateur a sélectionné des licences pour l’Audioconférence, Microsoft Teams et Skype Entreprise Online (plan 2).
    4. Les centres d'administration des utilisateurs cliquent sur **Afficher tout**, puis sur **Teams**.
    5. Dans le centre d’administration Microsoft Teams, cliquez sur **Portail hérité**.
    6. Dans le centre d’administration Skype Entreprise, cliquez sur **Audioconférence**, puis sur **Utilisateurs**.
    7. Sélectionnez l’utilisateur concerné et vérifiez que l’utilisateur dispose d’un numéro payant par défaut.

    Pour plus d’informations, consultez [Plans d’appels](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) ou appelez l’équipe de facturation Microsoft Commerce pour obtenir de l’aide sur les questions liées à la gestion des licences.

    Ressources supplémentaires

    - [Réunions et conférences dans Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audioconférence](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Stratégies de réunion** : les stratégies de réunion sont utilisées pour contrôler les fonctionnalités disponibles pour les participants aux réunions planifiées par les utilisateurs au sein de votre organisation. Après avoir créé une stratégie et apporté vos modifications, vous pouvez affecter des utilisateurs à la stratégie.

    - **Modifier ou créer une stratégie de réunion** : pour modifier ou créer une stratégie de réunion, accédez au **Centre d’administration Microsoft Teams > Réunions > Stratégies de réunion**. Sélectionnez une stratégie dans la liste ou cliquez sur **Ajouter**. Si vous créez une stratégie, ajoutez un nom et une description. Le nom ne peut pas contenir de caractères spéciaux et ne doit pas dépasser 64 caractères. Choisissez les paramètres, puis cliquez sur **Enregistrer**. 
    
        Par exemple, vous avez un grand nombre d’utilisateurs et vous voulez limiter la bande passante requise par la réunion. Vous devez créer une stratégie personnalisée nommée « bande passante limitée » et désactiver les paramètres suivants :

        Sous** Audio & vidéo** :
        - Désactivez **Autoriser l'enregistrement dans le cloud**.
        - Désactivez **Autoriser la vidéo IP**.

        Sous **Partage de contenu** :

        - Désactiver le mode de partage d’écran.
        - Désactivez **Autoriser le tableau blanc**.
        - Désactivez **Autoriser les notes partagées**.

        Puis, **attribuer la stratégie aux utilisateurs** :

    1. Dans le volet de navigation gauche du centre d’administration Microsoft Teams, accédez aux **Utilisateurs**, puis cliquez sur l’utilisateur.
    2. Sélectionnez l’utilisateur en cliquant à gauche du nom de celui-ci, puis cliquez sur **Modifier les paramètres**.
    3. Sous **Stratégie de réunion**, sélectionnez la stratégie que vous souhaitez attribuer, puis cliquez sur **Appliquer**.

    Pour attribuer une stratégie à plusieurs utilisateurs à la fois, consultez l’article [Modifier en masse les paramètres utilisateur Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Vous pouvez effectuer les opérations suivantes :
    1. Dans le volet de navigation gauche du centre d’administration Microsoft Teams, accédez aux **Réunions > Stratégies de réunion**.
    2. Sélectionnez la stratégie en cliquant à gauche du nom de celle-ci.
    3. Cliquez sur **Gérer les utilisateurs**.
    4. Dans le volet **Gérer les utilisateurs**, recherchez l’utilisateur par son nom complet ou son nom d’utilisateur, sélectionnez le nom, puis cliquez sur **Ajouter**. Répétez cette étape pour chaque utilisateur que vous souhaitez ajouter.
    5. Lorsque vous avez terminé d'ajouter les utilisateurs, cliquez sur **Enregistrer**.

- **Résoudre les problèmes liés à un pavé de numérotation manquant** :
    - Vérifiez qu’une [licence Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) a été attribuée à l’utilisateur.
    - Vérifiez qu’un [plan d’appel](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) a été attribué à l’utilisateur.
    - Activer les utilisateurs pour [Voix Entreprise](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Résoudre les problèmes de connexion de Teams** : Tout d’abord, vérifiez que le [service Microsoft Teams est sain](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Recherchez ensuite les codes d’erreur courants et consultez l’article [Pourquoi je n’arrive pas à me connecter à Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Vous pouvez également consulter l’article [Modèles d’identité et authentification dans Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
