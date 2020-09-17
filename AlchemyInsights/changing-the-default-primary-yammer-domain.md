---
title: Modifier le domaine Yammer par défaut
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 93c82b7e60838e0127062e8bf5ab394bb29650d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793864"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Modifier le domaine principal/par défaut de Yammer

L’URL de Yammer contient le nom de domaine principal actuel de votre réseau Yammer. Il se peut que ce nom de domaine ne corresponde pas au nom de domaine principal défini dans Office 365 ou Azure AD. Il existe certaines différences de comportement en fonction du nombre de domaines personnalisés ajoutés au client, et si Yammer est dans une configuration prise en charge (1 client : 1 réseau ou 1:1). Une documentation sur [Les domaines Yammer et Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) est disponible.

La raison la plus fréquente pour laquelle vous voyez un domaine incorrect est que plusieurs réseaux Yammer existent et ils doivent être consolidés. [La consolidation vers un réseau unique](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) en utilisant l’outil de migration réseau constitue une première étape importante. Effectuez cette opération avant de définir votre domaine principal.

**Aucun domaine personnalisé**

Pour les nouveaux clients, le domaine par défaut (par exemple, fabrikam.onmicrosoft.com) du client est utilisé pour Yammer. Le domaine principal est défini en tant que yammer.com/fabrikam.onmicrosoft.com.

**Domaine personnalisé unique**

Yammer sélectionne automatiquement le domaine personnalisé (par exemple, fabrikam.com) du client comme domaine principal dans Yammer. Il est défini en tant que yammer.com/fabrikam.com. Cette modification est apportée par le service de synchronisation de domaine et peut prendre jusqu’à 24 heures.

**Plusieurs domaines personnalisés**

Yammer peut avoir un domaine principal différent de celui du domaine par défaut du client. Comme il existe plusieurs domaines personnalisés, Yammer ne tente pas de deviner le domaine approprié parmi ceux disponibles. Vous devez ouvrir un cas de support technique pour demander que le nom de domaine principal soit remplacé par le domaine principal qui vous convient.

**Informations supplémentaires sur la résolution des problèmes**

Dans certains cas, les domaines peuvent avoir été déplacés parmi les clients et le service de synchronisation de domaines ne peut pas s’exécuter correctement. Il se peut que vous rencontriez des problèmes de connexion ou autres, outre le domaine principal incorrect. Pour résoudre ce problème, les domaines doivent être déplacés vers le réseau approprié avec l’Aide et support Microsoft. Cette situation nécessite une aide directe et sa résolution peut prendre du temps, en particulier si la liste de noms de domaine est très longue. Ouvrez un cas de support technique pour obtenir de l’aide sur la résolution de ce genre de problèmes.

Lorsque vous collaborez avec un agent du support, celui-ci vérifie, sous votre supervision, que les domaines sont vérifiés sur un client. Il peut vous poser des questions de vérification supplémentaires relatives à vos domaines s’ils sont ajoutés à votre client sans être vérifiés par DNS. Assurez-vous que les domaines sont vérifiés par DNS pour accélérer le processus.
