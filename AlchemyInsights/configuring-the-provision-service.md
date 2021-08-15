---
title: Configuration du service d’approvisionnement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033276"
---
# <a name="configuring-the-provision-service"></a>Configuration du service d’approvisionnement

Pour que la mise en service automatisée des utilisateurs fonctionne, Azure AD requiert des informations d’identification valides qui lui permettent de se connecter à l’API workday Web Services. En outre, le bouton Tester la connexion de l’application mise en service workday to AD permet également de vérifier s’il est en mesure de se connecter à l’agent d’approvisionnement Azure AD Connecter associé au domaine AD.

Si le portail Azure retourne une erreur lors de l’enregistrement des informations d’identification, suivez les étapes recommandées ci-dessous :

1. Confirmez que vous avez configuré le compte d’utilisateur du système d’intégration Workday comme indiqué dans la section didacticiel Configurer l’utilisateur du système [d’intégration dans Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Confirmez que le service Azure AD Connecter Provisioning Agent est opérationnel sur votre serveur Windows local à l’aide de la console de gestion des services. Vous pouvez également vérifier l’état de l’agent dans le portail Azure en cliquant sur le bouton Afficher les agents locaux.
3. Assurez-vous que vous entrez la valeur du champ « Nom d’utilisateur de la journée de travail » au format username@workday-tenant-name. Si le nom du client-jour est manquant, l’authentification Workday échoue.
4. Si vous configurez l’intégration avec le client d’implémentation Workday, notez les heures d’arrêt prévues de votre client Workday. Workday a programmé des temps d’arrêt pour ses locataires d’implémentation pendant les week-ends (généralement du vendredi soir au samedi matin) et les échecs de connectivité pendant cette fenêtre de temps d’arrêt sont un problème connu qui se résout automatiquement dès que les locataires d’implémentation sont de nouveau en ligne.
5. Dans de rares cas, vous pouvez également voir cette erreur si le mot de passe de l’utilisateur du système d’intégration a changé en raison de l’actualisation du client ou si le compte est dans un état verrouillé ou expiré. Vérifiez l’état de l’utilisateur du système d’intégration auprès de votre administrateur workday.

Pour d’autres détails sur la configuration de Workday pour l’approvisionnement automatique, voir [Tutoriel : Configurer Workday pour l'approvisionnement automatique d'utilisateurs](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
