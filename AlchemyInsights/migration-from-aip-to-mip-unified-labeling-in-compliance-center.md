---
title: Migrarea de la AIP la PMI/etichetarea unificată în centrul de conformitate
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674338"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrarea de la AIP la PMI/etichetarea unificată în centrul de conformitate

Pentru a migra de la etichetele AIP la etichetarea unificată în centrul de securitate și conformitate, procedați astfel:

**Activarea protecției din portalul Azure**

1. Dacă nu ați făcut deja acest lucru, deschideți o fereastră nouă de browser și [Conectați-vă la portalul Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navigați la lama de **protecție a informațiilor Azure** . De exemplu, în meniul hub, faceți clic pe **toate serviciile** și începeți să tastați **informații** în caseta de filtrare. Selectați **Azure Information Protection**. Dacă nu ați mai accesat lama Azure Information Protection înainte, consultați [pașii suplimentari](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pentru a adăuga această lamă la portal. Pentru a deschide lama Azure Information Protection, trebuie să aveți fie un [plan Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) , fie un plan 365 Office care include managementul drepturilor. Dacă aveți unul dintre aceste abonamente, dar vedeți un mesaj că nu se poate găsi un abonament valid, [contactați asistența Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) sau utilizați canalele de asistență standard.

2. Găsiți opțiunile de meniu **gestionare** și selectați **activare protecție**. Faceți clic pe **Activare**, apoi confirmați acțiunea. Când Activarea este finalizată, bara de informații afișează **Activarea terminată cu succes**.

**Migrarea etichetelor de protecție Azure Information la Office 365 Security & Conformity Center**

1. Asigurați-vă că sunteți conectat ca utilizator cu permisiunea de administrator global.

2. Navigați la lama de **protecție a informațiilor Azure** .

3. Din opțiunea **gestionare** meniu, selectați **etichetare unificată**.

4. În secțiunea **Azure Information Protection-lamă de etichetare unificată** , faceți clic pe **Activare** și urmați instrucțiunile online.

**Notă**: Verificați dacă aveți permisiunile corespunzătoare înainte de a activa migrarea în centrul de securitate & de conformitate. Consultați aceste articole pentru mai multe informații:

1. [Trebuie să fiți administrator global pentru a configura Azure Information Protection sau pot să delege altor administratori?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informații importante despre rolurile administrative după migrarea la centrul de conformitate & pentru securitate.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Pentru mai multe informații despre AIP la migrarea unificată a etichetelor către centrul de securitate și conformitate, consultați [migrarea etichetelor](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
