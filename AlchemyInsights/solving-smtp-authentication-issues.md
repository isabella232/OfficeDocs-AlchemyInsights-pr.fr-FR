---
title: Activer l'authentification et le dépannage SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321751"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Activer l'authentification et le dépannage SMTP

Si vous souhaitez activer l’authentification SMTP pour une boîte aux lettres ou si vous obtenez une erreur « Client non authentifié », « Échec de l’authentification » ou « SmtpClientAuthentication » avec le code 5.7.57 ou 5.7.3 ou 5.7.139 lorsque vous tentez de relayer le courrier en authentifiant un appareil ou une application avec Microsoft 365, effectuez ces trois actions pour résoudre le problème :

1. Désactivez [les valeurs par défaut de la sécurité d 'Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)en mettant l'option **Activer les valeurs par défaut** de la sécurité sur **Non**.

    a. Connectez-vous au portail Microsoft Azure en tant qu'administrateur de sécurité, administrateur d'accès conditionnel ou administrateur global.<BR/>
    b. Naviguez jusqu'à Azure Active Directory >  **Propriétés**.<BR/>
    c. Sélectionnez **Gérer les paramètres de sécurité par défaut**.<BR/>
    d. Définir **l'activation de la sécurité par défaut** sur **Non**.<BR/>
    e. Sélectionnez **Enregistrer**.

2. [Activez la soumission SMTP du client](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) sur la boîte aux lettres sous licence.

    a. Dans le centre d'administration de Microsoft 365, accédez à **Utilisateurs actifs** , puis sélectionnez l'utilisateur.<BR/>
    b. Allez dans l'onglet Courrier, et sous **Applications de messagerie**, sélectionnez **Gérer les applications** de messagerie.<BR/>
    d. Assurez-vous que la case **Authenticated SMTP** est cochée (activée).<BR/>
    e. Sélectionnez **Enregistrer les modifications**.<BR/>

3. [Désactiver l'authentification multifactorielle (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) sur la boîte aux lettres sous licence.

    a. Allez dans le centre d'administration de Microsoft 365, et dans le menu de navigation de gauche, sélectionnez **Utilisateurs** > **Utilisateurs actifs**.<BR/>
    b. Sélectionnez **Authentification multifactorielle**.<BR/>
    c. Sélectionnez l'utilisateur et désactivez **l'authentification multifactorielle**.<BR/>
