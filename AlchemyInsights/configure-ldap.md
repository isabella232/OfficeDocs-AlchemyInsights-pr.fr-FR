---
title: Configurer LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876548"
---
# <a name="configure-ldap"></a><span data-ttu-id="c04e7-102">Configurer LDAP</span><span class="sxs-lookup"><span data-stu-id="c04e7-102">Configure LDAP</span></span>

<span data-ttu-id="c04e7-103">Pour configurer LDAP, faites les choses suivantes :</span><span class="sxs-lookup"><span data-stu-id="c04e7-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="c04e7-104">Vérifiez l’état d’état de votre domaine sur [le portail Azure.](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="c04e7-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="c04e7-105">Assurez-vous qu’un abonnement Azure AD valide est disponible et que les services de domaine Azure AD ont été activés.</span><span class="sxs-lookup"><span data-stu-id="c04e7-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="c04e7-106">Le certificat requis pour activer le LDAP sécurisé doit être obtenu auprès d’une autorité de certification publique de confiance ou être un certificat auto-signé.</span><span class="sxs-lookup"><span data-stu-id="c04e7-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="c04e7-107">Assurez-vous que le certificat suit les [instructions requises.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)</span><span class="sxs-lookup"><span data-stu-id="c04e7-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="c04e7-108">**Certificat non valide**</span><span class="sxs-lookup"><span data-stu-id="c04e7-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="c04e7-109">Pour renouveler un certificat, suivez les étapes pour créer un certificat et recharger : [Configurez LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c04e7-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="c04e7-110">Pour résoudre le problème connu avec les alertes LDAP sécurisées dans Les services de domaine Azure Active Directory, consultez [Résoudre les alertes LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c04e7-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
