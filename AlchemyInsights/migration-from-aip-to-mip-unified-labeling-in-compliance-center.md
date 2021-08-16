---
title: Migrarea de la AIP la eticheta MIP/Unificată în Centrul de conformitate
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000368"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrarea de la AIP la eticheta MIP/Unificată în Centrul de conformitate

Pentru a migra de la etichete AIP la Etichetare unificată în Centrul de securitate și conformitate, efectuați următoarele:

**Activarea protecției din portalul Azure**

1. Dacă nu ați făcut deja acest lucru, deschideți o fereastră nouă de browser [și conectați-vă la portalul Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Navigați la **blade Azure Information Protection.** De exemplu, în meniul hub, faceți clic **pe Toate serviciile** și începeți să **tastați** Informații în caseta Filtrare. Selectați **Azure Information Protection.** Dacă nu ați accesat înainte sistemul blade Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection, consultați pașii suplimentari pentru adăugarea acestui blade în portal. Pentru a deschide azure information protection, trebuie să aveți un [plan Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) sau un plan Office 365 care include Rights Management. Dacă aveți unul dintre aceste abonamente, dar vedeți un mesaj care spune că nu poate fi găsit un abonament valid, [contactați](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) Asistența Microsoft sau utilizați canalele de asistență standard.

2. Găsiți **opțiunile** din meniul Gestionare și selectați **Activare protecție.** Faceți **clic** pe Activare , apoi confirmați acțiunea. Atunci când activarea s-a terminat, bara de informații afișează **Activarea s-a finalizat cu succes.**

**Migrarea etichetelor Azure Information Protection la Centrul Office 365 securitate & conformitate**

1. Asigurați-vă că sunteți conectat ca utilizator cu permisiunea Administrator global.

2. Navigați la **blade Azure Information Protection.**

3. Din opțiunea **de** meniu Gestionare, **selectați Etichetare unificată**.

4. Pe **Azure Information Protection - etichetare unificată** blade, faceți clic pe **Activare și** urmați instrucțiunile online.

**Notă:** Verificați dacă aveți permisiunile corespunzătoare înainte de a activa Migrarea Centrului & de conformitate. Consultați aceste articole pentru mai multe informații:

1. [Trebuie să fiți administrator global pentru a configura Azure Information Protection sau pot delega altor administratori?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informații importante despre rolurile administrative după migrarea la Centrul de & conformitate.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Pentru mai multe informații despre AIP la Centrul unificat de etichetare a migrării la Centrul de securitate și conformitate, consultați [Migrarea etichetelor.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
