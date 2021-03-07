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
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430743"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="a5006-102">Configurer le service de synchronisation MIM</span><span class="sxs-lookup"><span data-stu-id="a5006-102">Configure MIM Sync service</span></span>

<span data-ttu-id="a5006-103">Le service de synchronisation Microsoft Identity Manager (MIM) est un composant de MIM.</span><span class="sxs-lookup"><span data-stu-id="a5006-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="a5006-104">Il s’agit d’un service local centralisé qui stocke et intègre des informations pour les organisations qui ont plusieurs annuaires et bases de données locaux.</span><span class="sxs-lookup"><span data-stu-id="a5006-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="a5006-105">Vous pourrez peut-être résoudre votre problème avec la synchronisation MIM si le problème a été résolu dans une mise à jour récente de MIM ou s’il s’agit de l’un des autres problèmes mentionnés dans la section ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a5006-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="a5006-106">**Étapes recommandées**</span><span class="sxs-lookup"><span data-stu-id="a5006-106">**Recommended steps**</span></span>

1. <span data-ttu-id="a5006-107">Vérifiez que vous utilisez une mise à jour récente de la synchronisation MIM et consultez les [Notes de publication de la synchronisation MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) pour déterminer si le problème a été résolu dans une mise à jour.</span><span class="sxs-lookup"><span data-stu-id="a5006-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="a5006-108">Si le problème est celui du connecteur Generic LDAP, Generic SQL, Lotus Domino ou Web Services, assurez-vous que vous utilisez une mise à jour récente des [connecteurs génériques](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="a5006-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="a5006-109">Si une opération de synchronisation MIM s’arrête avec une erreur, consultez la table des [codes d'erreur d'exécution](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) pour déterminer les causes potentielles.</span><span class="sxs-lookup"><span data-stu-id="a5006-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="a5006-110">Si l’exécution s’arrête avec **extension-dll-exception**, cliquez sur ces mots pour ouvrir la fenêtre **Propriétés d’objet d’espace de connecteur**, puis cliquez sur **Trace de pile...** pour voir plus d’informations sur la cause sous-jacente, comme décrit dans [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="a5006-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="a5006-111">Si le service de notification de modification de mot de passe (PCNS) signale une **erreur 6025** dans le journal des événements pendant la synchronisation de mot de passe, consultez le guide de résolution des problèmes [Erreur de signalement au PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="a5006-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="a5006-112">Si la synchronisation complète avec l’agent de gestion des services FIM est lente, vérifiez le paramètre **auto grow** de TempDB, comme décrit dans [Résolution des problèmes de synchronisation complète lente ou suspendu](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="a5006-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="a5006-113">Si vous rencontrez une erreur « Serveur arrêté » dont la création a échoué via des services web à l’aide de l’agent de gestion des services FIM, consultez [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) pour une vue d’ensemble des causes.</span><span class="sxs-lookup"><span data-stu-id="a5006-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

