---
title: Facturare pentru achiziționarea de instanțe rezervate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823167"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturare pentru achiziționarea de instanțe rezervate

Achiziționarea de instanțe rezervate este taxată la metoda de plată legată de abonamentul pe care îl selectați în momentul achiziției. Tipul de abonament trebuie să fie un acord de întreprindere (număr ofertă: MS-AZR-0017P), Pay-as-you-go (număr ofertă: MS-AZR-0003P), Microsoft Customer Agreement sau CSP.

- Pentru un abonament pentru întreprinderi, tarifele sunt deduse din soldul angajamentului monetar al înscrierii sau sunt percepute ca supra-
- Pentru abonamentul pay-as-Go, tarifele sunt facturate pe cardul de credit sau pe metoda de plată a facturii în abonament

**Anularea rezervării**

- **Cu** autoservire: Puteți să anulați sau să schimbați singur o instanță rezervată utilizând [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervarea și faceți clic pe rambursare sau pe Exchange. Rețineți că trebuie să aveți acces proprietar în ordinea rezervării, pentru a face schimb sau a rambursa. Accesul la rezervare nu vă va permite să continuați cu rambursarea sau schimbul. Solicitați proprietarului comenzii de rezervare să vă ofere accesul proprietarului la comanda de rezervare
- **Politica Exchange:** Puteți face schimb de rezervări pentru o altă rezervare de același tip – nu există **penalități** la schimbul de rezervări. Angajamentul total al rezervării noi ar trebui să fie mai mare decât suma rambursată a rezervării și a plăților lunare viitoare (dacă este cazul)
- **Politica de rambursare:** Suma restituirilor și plățile viitoare anulate nu pot depăși $50.000 USD într-o fereastră rulantă de 12 luni. **În prezent nu percepem nicio sancțiune** pentru rambursări, dar o putem percepe pentru rambursări viitoare

**Excepții:** Capacitățile Exchange și anulare cu autoservire nu sunt disponibile pentru clienții din acordul de întreprindere guvernamentală din S.U.A.

- Asistența **API/PS/CLI** nu este disponibilă pentru anularea și rambursarea [schimburilor și restituirilor cu autoservire pentru rezervări Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Capacitățile Exchange și anulare cu autoservire nu sunt disponibile pentru clienții din acordul de întreprindere guvernamentală din SUA. Alte tipuri de abonamente pentru instituții guvernamentale din SUA, inclusiv plățile în timp și CSP sunt acceptate

Aflați mai multe: modul în care [sunt prelucrate tranzacțiile de returnare și Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Aflați mai multe [:](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) [Politica de schimb și de rambursare](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) alte întrebări

**Schimbul unei instanțe rezervate existente (cu autoservire)**

Puteți face schimb de rezervări pentru o altă rezervare de același tip. De asemenea, puteți să returnați o rezervare, de până la $50.000 USD pe an, dacă nu mai aveți nevoie de el. Capacitățile Exchange și anulare cu autoservire nu sunt disponibile pentru clienții din acordul de întreprindere guvernamentală din SUA. Alte tipuri de abonamente pentru guvern din SUA, inclusiv plățile în timp și CSP, sunt acceptate. Trebuie să aveți acces proprietar în ordinea rezervării pentru a face schimb de taxe sau pentru a rambursa o rezervare existentă.

Următorii pași vor ghida procedura de terminare a tranzacției

1. Conectați-vă la [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervările pe care doriți să le rambursați și faceți clic pe **Exchange** 2. Selectați produsul VM pe care doriți să-l achiziționați și tastați o cantitate. Asigurați-vă că noul total de achiziție este mai mare decât totalul de returnare [determină dimensiunea potrivită înainte](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)de a cumpăra.
3. revizuiți și Finalizați tranzacția

**Rambursarea unei instanțe rezervate**

Pentru a rambursa o rezervare, accesați **detaliile rezervării** și faceți clic pe **rambursare**

**Rambursare pro-nominală:**

**Exemple Pro-rație și cerințe minime pentru rambursare și Exchange** Exemplu de rezervare în avans:

- Achiziționați un termen de un an RI pentru $120 pe 1 ianuarie
- Pe 7 aprilie doriți să returnați sau să schimbați această rezervare
- Deoarece rezervarea a fost în direct pentru 97 de zile, veți primi (1-97/365) * $120 înapoi. (de exemplu, $88,1). În prezent nu există nicio sancțiune pentru rambursări
- Dacă faceți schimb de focuri, noua achiziție trebuie să fie mai mare decât $88,1
- Nu există nicio sancțiune în ceea ce privește rambursările în prezent

**Exemplu de rezervare a planului de facturare:**

- Achiziționați un termen de un an RI pentru $10 pe lună
- Pe 7 aprilie doriți să returnați sau să schimbați această rezervare
- Deoarece ultima plată a avut loc 7 zile, veți primi (1-7/31) * $10 înapoi. (de exemplu, $7,74)
- Plățile viitoare anulate sunt $80. În prezent nu există nicio sancțiune pentru rambursări
- Această anulare va deduce $87,74 de la dumneavoastră sunteți limita de rambursare $50.000
- Dacă faceți schimb de valori, valoarea totală a achiziției noi trebuie să fie mai mare decât $87,74

**Nu se poate vedea factură pentru ultima perioadă de facturare**

Unele motive posibile este posibil să nu vedeți o factură:

- Aveți o sumă lunară de credit cu abonamentul pe care nu l-ați depășit sau aveți o versiune de încercare gratuită. O factură este generată numai atunci când datorați bani
- Sunt mai puțin de 30 de zile de la data la care v-ați abonat la Azure
- Factura nu este generată încă. Așteptați până la sfârșitul perioadei de facturare
- Dacă nu sunteți administrator de cont, este posibil ca facturile mai vechi să nu fie disponibile pentru dvs.

**Descărcarea facturii din Azure portal (. pdf)**

- Selectați abonamentul din pagina [abonamente](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) din Azure portal ca [utilizator cu acces la facturi](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selectați **facturi**
- Faceți clic pe **Descărcare factură** pentru a vizualiza o copie a facturii PDF. Dacă acesta spune **nu este disponibil** , consultați [de ce nu văd o factură pentru ultima perioadă de facturare?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Primirea facturii prin e-mail (. pdf)**

- Selectați abonamentul din pagina [abonamente](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Faceți clic pe **facturi** apoi trimiteți prin e-mail factura mea
- Faceți clic pe **înscriere** și acceptați termenii. Va trebui să optați pentru fiecare abonament pe care îl dețineți

Notă: dacă nu primiți un e-mail după ce urmați pașii, asigurați-vă că adresa de e-mail este corectă în [preferințele de comunicare din profilul dvs](https://account.windowsazure.com/profile) .

**Descărcarea datelor de utilizare din portalul Azure**

- Conectați-vă la [Centrul de cont Azure](https://account.windowsazure.com/Subscriptions) ca [administrator de cont](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selectați abonamentul pentru care doriți informațiile despre factură și utilizare
- Selectați **istoricul de facturare**
- Selectați **vedeți instrucțiunea curentă** pentru a vedea o estimare a taxelor în momentul în care a fost generată estimarea
- Selectați **Descărcare utilizare** pentru a descărca datele de utilizare zilnică ca fișier CSV. Dacă vedeți două versiuni disponibile, descărcați versiunea 2

Alte întrebări: [accesați documentele de instanță rezervate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documente recomandate**

- [Noțiuni de bază despre facturare](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegerea modului în care se aplică reducerea instanței rezervate](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Descărcarea sau vizualizarea facturii de facturare Azure și a datelor de utilizare zilnică](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegerea modului în care se aplică reducerea instanței rezervate](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegerea utilizării de exemplu rezervat pentru abonamentul cu plată-ca-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegerea utilizării instantei rezervate pentru înscrierea întreprinderii](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Costurile software-ului Windows nu sunt incluse în instanțele rezervate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instanțe rezervate în Programul Partner central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)