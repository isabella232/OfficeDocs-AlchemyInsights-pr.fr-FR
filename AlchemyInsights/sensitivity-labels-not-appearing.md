---
title: Étiquettes de sensibilité non affichées
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048650"
---
# <a name="sensitivity-labels-not-appearing"></a>Étiquettes de sensibilité non affichées

Les étiquettes de sensibilité vous permettent de classer et de protéger votre contenu sensible. Elles peuvent être créées dans le centre de conformité Microsoft 365, le centre de sécurité Microsoft 365 ou le centre de sécurité & de sécurité Office 365 sous classification > les étiquettes de sensibilité. Pour en savoir plus sur cette fonctionnalité, reportez-vous à la rubrique [vue d’ensemble des étiquettes de confidentialité](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Si vous avez configuré vos étiquettes de confidentialité mais qu’elles n’apparaissent pas dans les applications Office, vérifiez les points suivants :

- Vérifiez que l’étiquette de confidentialité a été [publiée](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) sur les utilisateurs et les groupes que vous souhaitez.

- Vérifiez que l’utilisateur utilise une application qui prend en charge les étiquettes de confidentialité-voir [étiquettes de confidentialité dans votre document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Si vous [migrez des étiquettes Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), tenez compte des considérations indiquées [ici](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Prise en charge de la protection contre la perte de données (DLP) : actuellement, seules les étiquettes de rétention peuvent être utilisées comme condition dans les stratégies DLP.  La prise en charge des étiquettes de sensibilité dans une stratégie DLP n’est pas encore disponible, mais nous y travaillons.

- Lorsque le chiffrement est activé sur une étiquette de sensibilité, vous pouvez choisir l’une des actions suivantes :
    - Attribuer des autorisations maintenant
    - Permettre aux utilisateurs d’attribuer des autorisations


Pour plus d’informations sur les problèmes éventuels, reportez-vous à [problèmes connus avec les étiquettes de confidentialité](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).