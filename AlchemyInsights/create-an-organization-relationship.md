---
title: Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854016"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation

1. À partir du tableau de bord du Centre d’administration Microsoft 365, accédez à **Administrateur** > ** Exchange**.
2. Accédez à **organisation** > **partage**.
3. Sous **Partage d’organisation**, cliquez sur **Nouveau**.
4. Dans **Nouvelle relation organisationnelle**, dans la boîte de dialogue **Nom de la relation**, entrez un nom convivial pour la relation d'organisation.
5. In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars. If you need to enter more than one domain, separate the domain names with a comma. For example, contoso.com, service.contoso.com.
6. Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.  

Pour définir le niveau d'accès de la disponibilité, sélectionnez l'une des opérations suivantes :

- **Informations de disponibilité de calendrier avec les heures de disponibilité uniquement**
- **Disponibilité de calendrier avec l’heure, l'objet et emplacement**  

 Pour définir les utilisateurs qui partagent des informations de disponibilité de calendrier, sélectionnez l'une des options suivantes :

- **Tout le monde dans votre organisation**
- **Un groupe de sécurité spécifié**  

Cliquez sur **Parcourir** pour sélectionner un groupe de sécurité dans la liste, puis cliquez sur **OK**.

Cliquez sur **Enregistrer** pour créer la relation organisationnelle.  

**Remarque :** les configurations inter-clients ne prennent pas en charge les contacts personnels pour la recherche de disponibilité. Vous devez inclure les contacts dans la liste d’adresses globale pour que la recherche de disponibilité fonctionne.

**Pour une compréhension complète de ce sujet, veuillez consulter :**

- [Créer une relation d’organisation dans Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [Modifier une relation d’organisation dans Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [Supprimer une relation d’organisation dans Exchange Online](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
