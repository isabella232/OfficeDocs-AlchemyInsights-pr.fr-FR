---
title: L’accès conditionnel avec un appareil joint au domaine me bloque
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: d71bb376615191f507d39b99d9e51ca77d929b90
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323436"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>L’accès conditionnel avec un appareil joint au domaine me bloque

**Outils hautement recommandés**

[Outil de résolution des problèmes d’alignement des appareils](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) : outil qui vous aide à résoudre les problèmes les plus courants d’alignement des appareils.

[Script de connectivité pour l'alignement des appareils de test](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : script contribuant à garantir qu’un appareil peut accéder aux points de terminaison d’alignement des appareils sous le compte système.

[Script de nettoyage d’appareil Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : script qui vous permet de rechercher, puis de gérer les appareils obsolètes dans votre environnement.

Voici quelques-unes des raisons courantes pour lesquelles l’accès conditionnel peut échouer sur un appareil qui a rejoint un domaine (Azure AD Hybride).

1. **Il n’y a pas de PRT Azure AD sur votre appareil** Vous devez vous assurer que l’appareil a le jeton d’actualisation principal (PRT) Azure AD (PRT). Pour plus d’informations sur PRT, consultez ce [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Pour vérifier si vous avez le jeton d’actualisation principal Azure AD, vous pouvez exécuter la commande `dsregcmd/status` sur l’appareil, puis vérifier si « AzureAdPrt » a la valeur « YES ».

Si « AzureAdPrt » a la valeur « NO », vérifiez les points suivants :

- **Si vous avez un environnement fédéré avec AD FS et qu’il est inaccessible aux réseaux d’accueil de vos utilisateurs** : dans ce cas, vérifiez que vos points de terminaison « usernamemixed » sont accessibles depuis l’extranet. Si votre service AD FS se trouve derrière un VPN, vérifiez que les utilisateurs se connectent au VPN, puis se connectent de nouveau à l’appareil. Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Déterminer si le module de plateforme sécurisée de l’appareil est défectueux et ne peut donc pas authentifier l’appareil** : vérifiez « tpm.msc » pour déterminer si l’état du l’appareil est « Prêt ». Si ce n’est pas le cas, exécutez `dsregcmd/leave`, puis laissez l’appareil se joindre de nouveau à Azure AD. Réessayez ensuite. Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Vous utilisez un fournisseur d’identité tiers, qui ne prend pas en charge les protocoles WS-Trust**. Comme décrit dans nos documents, les appareils joints à Azure AD Hybride ne peuvent pas fonctionner dans ce cas. Veuillez contacter votre fournisseur d’identité pour obtenir du support.

2. **Les utilisateurs utilisent le navigateur Chrome sans les comptes Windows 10** ou **l’extension Office Chrome n’utilise pas automatiquement le jeton d’actualisation principal sur des appareils joints à AAD ou AAD Hybride** : cela entraîne l’échec de toutes les stratégies d’accès conditionnel basées sur les appareils, avec le message d’erreur « Appareil non inscrit » affiché. Pour utiliser correctement le navigateur Chrome, vous devez installer les « comptes Windows 10 » ou « l'extension d’Office au navigateur Chrome des utilisateurs » via SCCM ou Intune. Si vous souhaitez en savoir plus, veuillez consulter ce [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

S’il n’est pas possible d’envoyer (push) l’extension à distance, dites aux utilisateurs d’installer manuellement l’une des extensions ci-dessus pour accéder aux applications derrière l’accès conditionnel basé sur l’appareil. Pour plus d’informations, consultez ce [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Vous avez correctement joint l’appareil à Azure AD Hybride, mais vous l’avez supprimé ou désactivé par inadvertance, en raison de modifications de synchronisation dans Azure AD Connect ou depuis le portail Azure** : dans ce cas, le programme ne reconnaît plus l’objet de l’appareil comme un appareil complètement joint, même si les statuts « AzureAdJoined » et « PRT » apparaissent comme valides sur l’appareil.

Pour résoudre ce problème, exécutez `dsregcmd/leave` sur les appareils affectés et laissez-les rejoindre Azure AD. Pour plus d’informations, consultez cette ce [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

**Remarque**: Si vos appareils sont sous Windows 10, mise à jour 1809, avec un proxy VPN/cloud et que vous voyez des problèmes d’état «AzureAdPrt» ou toute application avec un problème d'authentification unique (Outlook ne se connecte pas à la boîte aux lettres même si vous aviez un jeton d’actualisation principal), vérifiez que vous avez ce correctif [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ou la mise à jour cumulative d’avril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) pour éviter les défaillances du jeton d’actualisation principal sur ces ordinateurs.

















