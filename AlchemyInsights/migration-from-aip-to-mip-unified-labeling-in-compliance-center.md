---
title: Migration des étiquettes AIP vers un étiquetage unifié/MIP dans le Centre de conformité
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236436"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migration des étiquettes AIP vers un étiquetage unifié/MIP dans le Centre de conformité

Pour migrer des étiquettes AIP vers un étiquetage unifié dans le Centre de sécurité et de conformité, procédez comme suit :

**Activer la protection à partir du portail Azure**

1. Si vous ne l’avez pas encore fait, ouvrez une nouvelle fenêtre de navigateur et [Connectez-vous au portail Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Accédez au panneau **Azure Information Protection**. Par exemple, dans le menu hub, cliquez sur **Tous les services** et commencez à taper **Informations** dans la zone de filtre. Sélectionnez **Azure Information Protection**. Si vous n’avez pas jamais accédé au panneau Azure Information Protection, consultez les [étapes supplémentaires](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pour l’ajouter au portail. Pour ouvrir le panneau d’Azure Information Protection, vous devez disposer d’un plan [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou d’une offre Office 365 incluant Rights Management. Si vous avez l’un de ces abonnements, mais que vous voyez un message indiquant qu’un abonnement valide est introuvable, [Contacter l’Aide et support Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ou utiliser vos canaux de support standard.

2. Recherchez les options du menu **Gérer**, puis sélectionnez **activation de la protection**. Cliquez sur **Activer**, puis confirmez votre action. Une fois l’activation terminée, la barre d’informations affiche **L’activation s’est correctement terminée**.

**Migrer des étiquettes Azure Information Protection vers le Centre de sécurité et conformité Office 365**

1. Vérifiez que vous êtes connecté en tant qu’utilisateur disposant des autorisations d’administrateur général.

2. Accédez au panneau **Azure Information Protection**.

3. À partir de l’option de menu **Gérer**, sélectionnez **Étiquetage unifié**.

4. Sur le panneau **Azure Information Protection – Étiquetage unifié**, cliquez sur **Activer** et suivez les instructions en ligne.

**Remarque**: Vérifiez que vous disposez des autorisations appropriées avant d’activer la migration du Centre de sécurité et conformité. Pour plus d’informations, voir les articles suivants :

1. [Est-ce que je dois être un administrateur général pour configurer Azure Information Protection, ou puis-je déléguer aux autres administrateurs ?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informations importantes sur les rôles d’administrateur après la migration vers le Centre de sécurité et conformité.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Pour plus d’informations sur la migration des AIP vers l’étiquetage unifié dans le Centre de sécurité et conformité, voir [Migrer des étiquettes](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
