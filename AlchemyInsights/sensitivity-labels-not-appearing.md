---
title: Étiquettes de niveau de sensibilité qui n’apparaissent pas
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061430"
---
# <a name="sensitivity-labels-not-appearing"></a>Étiquettes de niveau de sensibilité qui n’apparaissent pas

Les étiquettes de sensibilité vous permettent de classer et de protéger votre contenu sensible. Ils peuvent être créés dans le centre de sécurité Centre de conformité Microsoft 365, Microsoft 365 ou le Centre de sécurité Microsoft 365 et conformité & sous les étiquettes de niveau de > classification. Pour en savoir plus sur cette fonctionnalité, voir [Vue d’ensemble des étiquettes de sensibilité.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Si vous avez configuré vos étiquettes de sensibilité, mais qu’elles n’apparaissent pas dans les applications Microsoft 365, vérifiez les questions suivantes :

- Confirmez que l’étiquette de niveau de sensibilité a [été](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) publiée pour les utilisateurs et les groupes que vous souhaitez.

- Confirmez que l’utilisateur utilise une application qui prend en charge les étiquettes de sensibilité : consultez les étiquettes de [sensibilité dans votre document.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Si vous migrez [des étiquettes Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)n’ignorez pas les considérations répertoriées [ici.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Prise en charge de la protection contre la perte de données (DLP) : actuellement, seules les étiquettes de rétention peuvent être utilisées comme condition dans les stratégies DLP.  La prise en charge des étiquettes de confidentialité dans une stratégie DLP n’est pas encore disponible, mais nous y travaillons.

- Lorsque le chiffrement est activé sur une étiquette de niveau de sensibilité, vous pouvez choisir l’une ou l’autre des façons de :
    - Attribuer des autorisations maintenant
    - Permettre aux utilisateurs d’attribuer des autorisations


Pour plus d’informations sur les problèmes possibles, voir [Problèmes connus avec les étiquettes de sensibilité.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)