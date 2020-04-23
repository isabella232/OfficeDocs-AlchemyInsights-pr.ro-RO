---
title: Notificări de alertă SharePoint nu sunt livrate
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742059"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Notificări de alertă SharePoint nu sunt livrate

Verificați folderul JUNK din e-mail, deoarece uneori alertele ar putea merge acolo.

Determinați dacă **toate avertizările nu sunt livrate** sau dacă nu este **livrată o avertizare individuală** dintr-un anumit fișier sau bibliotecă.

- **Alerte individuale nu sunt livrate:** Dacă o avertizare individuală dintr-un anumit fișier sau bibliotecă nu este livrată, puteți încerca să o ștergeți și să o creați din nou. Consultați [Gestionarea, vizualizarea sau ștergerea alertelor SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) pentru a recrea alerta.
- **Toate alertele nu sunt livrate:** Dacă nu sunt livrate toate alertele din mai multe fișiere sau biblioteci, vizitați [tabloul de bord Sănătate serviciu](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a verifica orice recomandări/incidente care pot apărea cu SharePoint sau Exchange. Problema ar putea fi cu capacitatea de alertă SharePoint sau întârzieri în e-mailuri prin Exchange. De asemenea, va fi important să rețineți dacă alte e-mail este livrat, și dacă nu, problema este probabil cu întârzieri Exchange.

Întrebări frecvente despre alerte:

- Nu este posibil să trimiteți alerte grupului de distribuire, sunt acceptate numai grupurile Security și O365.
- Nu aveți posibilitatea să particularizați șabloanele de e-mail de avertizare; trebuie să utilizați Fluxul de lucru Microsoft FLOW sau SharePoint Designer pentru a le atinge.

Mai multe informații:

- **Configurare a alertei**: Pentru mai multe informații despre configurarea avertizărilor, consultați [Crearea unei alerte pentru a fi notificată atunci când un fișier sau un folder se modifică în SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Depanarea avertizărilor**: Pentru mai multe informații despre depanarea avertizărilor, consultați [Utilizatorii nu primesc notificări de avertizare SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Politici avansate de alertă de conformitate O365:** Pentru mai multe informații despre configurarea acestor alerte, consultați [Politicile de alertă de conformitate](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **Jurnalele de audit SharePoint și OneDrive:** Pentru mai multe informații despre să regăsiți aceste evenimente, consultați [Căutarea jurnalului de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Alerte trimise de Protecție avansată a amenințărilor:** Consultați [ATP pentru SharePoint și OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Alerte trimise de poliția de prevenire a pierderilor de date:** Consultați [notificările prin e-mail pentru politicile DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Subiecte înrudite

Doriți să încercați Microsoft Flow în SharePoint Online?

- [Creare flux](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint și Flux](https://flow.microsoft.com//blog/sharepoint-and-flow/)
