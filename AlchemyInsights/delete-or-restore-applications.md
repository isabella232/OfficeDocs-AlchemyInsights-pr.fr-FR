---
title: Supprimer ou restaurer des applications
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102569"
---
# <a name="delete-or-restore-applications"></a>Supprimer ou restaurer des applications

**Pour supprimer une application de votre client Azure AD**:

1. Dans le **portail Azure AD,** sélectionnez **Enterprise applications.** Recherchez et sélectionnez ensuite l’application à supprimer.
2. Dans la section **Gérer** dans le volet gauche, sélectionnez **Propriétés.**
3. Sélectionnez Supprimer, puis **Oui** pour confirmer la suppression de l’application de votre client Azure AD. 

Pour plus d’informations sur la suppression d’une application, voir Démarrage rapide : supprimer une application de [Azure Active Directory client (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

Dans PowerShell, la cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) supprime les configurations de proxy d’application d’une application spécifique dans Azure Active Directory et peut supprimer complètement l’application si elle est spécifiée.

Vous pouvez **restaurer une application supprimée à l’aide** de PowerShell. Une fois que l’application que vous souhaitez restaurer a été identifiée, vous pouvez la restaurer à l’aide [de Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
