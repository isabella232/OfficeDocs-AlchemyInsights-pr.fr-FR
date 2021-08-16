---
title: Configurer le service de synchronisation MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978483"
---
# <a name="configure-mim-sync-service"></a>Configurer le service de synchronisation MIM

Le service de synchronisation Microsoft Identity Manager (MIM) est un composant de MIM. Il s’agit d’un service local centralisé qui stocke et intègre des informations pour les organisations qui ont plusieurs annuaires et bases de données locaux. Vous pourrez peut-être résoudre votre problème avec la synchronisation MIM si le problème a été résolu dans une mise à jour récente de MIM ou s’il s’agit de l’un des autres problèmes mentionnés dans la section ci-dessous.

**Étapes recommandées**

1. Vérifiez que vous utilisez une mise à jour récente de la synchronisation MIM et consultez les [Notes de publication de la synchronisation MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) pour déterminer si le problème a été résolu dans une mise à jour.
2. Si le problème est celui du connecteur Generic LDAP, Generic SQL, Lotus Domino ou Web Services, assurez-vous que vous utilisez une mise à jour récente des [connecteurs génériques](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Si une opération de synchronisation MIM s’arrête avec une erreur, consultez la table des [codes d'erreur d'exécution](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) pour déterminer les causes potentielles.
4. Si l’exécution s’arrête avec **extension-dll-exception**, cliquez sur ces mots pour ouvrir la fenêtre **Propriétés d’objet d’espace de connecteur**, puis cliquez sur **Trace de pile...** pour voir plus d’informations sur la cause sous-jacente, comme décrit dans [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Si le service de notification de modification de mot de passe (PCNS) signale une **erreur 6025** dans le journal des événements pendant la synchronisation de mot de passe, consultez le guide de résolution des problèmes [Erreur de signalement au PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Si la synchronisation complète avec l’agent de gestion des services FIM est lente, vérifiez le paramètre **auto grow** de TempDB, comme décrit dans [Résolution des problèmes de synchronisation complète lente ou suspendu](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Si vous rencontrez une erreur « Serveur arrêté » dont la création a échoué via des services web à l’aide de l’agent de gestion des services FIM, consultez [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) pour une vue d’ensemble des causes.

