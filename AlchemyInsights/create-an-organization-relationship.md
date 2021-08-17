---
title: Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation
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
- "3800014"
- "898"
ms.openlocfilehash: 5ea0f3dd2c1e21455b4750afbf9c43c931ad34bf357e94dd604ffe5bcdd2fa64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080348"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>Créer une relation d’organisation pour permettre à vos utilisateurs de collaborer avec une autre organisation

1. À partir du tableau de bord du Centre d’administration Microsoft 365, accédez à **Administrateur** > **Exchange**.
2. Accédez à **organisation** > **partage**.
3. Sous **Partage d’organisation**, cliquez sur **Nouveau**.
4. Dans **Nouvelle relation organisationnelle**, dans la boîte de dialogue **Nom de la relation**, entrez un nom convivial pour la relation d'organisation.
5. Dans la zone **Domaines à partager avec**, tapez le domaine de l'organisation Office 365 externe ou Exchange sur site à laquelle vous voulez donner accès à vos calendriers. Pour entrer plusieurs domaines, séparez les noms de domaine par une virgule. Par exemple, contoso.com, service.contoso.com.
6. Cochez la case **Activer le partage des informations de disponibilité de calendrier** pour activer le partage de calendrier avec les domaines que vous avez répertoriés. Définissez le niveau de partage des informations de disponibilité du calendrier, ainsi que les utilisateurs pouvant partager ces informations.  

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
