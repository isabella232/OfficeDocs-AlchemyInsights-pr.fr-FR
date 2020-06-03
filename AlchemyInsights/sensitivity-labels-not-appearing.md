---
title: Étiquettes de sensibilité non affichées
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 1326eca02044014a8e9c072fcc3e4cd3a41c7a9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511650"
---
# <a name="sensitivity-labels-not-appearing"></a>Étiquettes de sensibilité non affichées

Les étiquettes de sensibilité vous permettent de classer et de protéger votre contenu sensible. Elles peuvent être créées dans le centre de conformité Microsoft 365, le centre de sécurité Microsoft 365 ou le centre de sécurité & Microsoft 365 Security Security Center sous classification > labels de sensibilité. Pour en savoir plus sur cette fonctionnalité, reportez-vous à la rubrique [vue d’ensemble des étiquettes de confidentialité](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Si vous avez configuré vos étiquettes de confidentialité mais qu’elles n’apparaissent pas dans les applications Office, vérifiez les points suivants :

- Vérifiez que l’étiquette de confidentialité a été [publiée](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) sur les utilisateurs et les groupes que vous souhaitez.

- Vérifiez que l’utilisateur utilise une application qui prend en charge les étiquettes de confidentialité-voir [étiquettes de confidentialité dans votre document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Si vous [migrez des étiquettes Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), tenez compte des considérations indiquées [ici](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Prise en charge de la protection contre la perte de données (DLP) : actuellement, seules les étiquettes de rétention peuvent être utilisées comme condition dans les stratégies DLP.  La prise en charge des étiquettes de sensibilité dans une stratégie DLP n’est pas encore disponible, mais nous y travaillons.

- Lorsque le chiffrement est activé sur une étiquette de sensibilité, vous pouvez choisir l’une des actions suivantes :
    - Attribuer des autorisations maintenant
    - Permettre aux utilisateurs d’attribuer des autorisations


Pour plus d’informations sur les problèmes éventuels, reportez-vous à [problèmes connus avec les étiquettes de confidentialité](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).