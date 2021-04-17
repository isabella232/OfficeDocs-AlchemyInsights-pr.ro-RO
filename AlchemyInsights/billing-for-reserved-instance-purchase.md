---
title: Facturare pentru achiziția de instanță rezervată
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820334"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturare pentru achiziția de instanță rezervată

Achiziția instanței rezervate este debitată la metoda de plată legată la abonamentul pe care îl selectați în momentul achiziției. Tipul de abonament trebuie să fie un contract de întreprindere (numărul ofertei: MS-AZR-0017P), Pay-As-You-Go (număr de ofertă: MS-AZR-0003P), Contractul pentru clienți Microsoft sau CSP.

- Pentru un abonament la nivel de întreprindere, taxele sunt scăzute din soldul angajamentului monetar al înscrierii sau din suma percepută ca supraabonare
- Pentru abonamentul Pay-As-You-Go, taxele sunt facturate pe cardul de credit sau prin factură, în abonamentul

**Se anulează rezervarea**

- **Autoserviție:** Puteți să anulați sau să schimbați singur o instanță rezervată [utilizând portalul Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Selectați rezervarea și faceți clic pe rambursare sau pe schimb. Rețineți că trebuie să aveți acces ca proprietar în Comanda de rezervare pentru schimb sau rambursare. Accesul doar la Rezervare nu vă va permite să continuați cu rambursarea sau schimbul. Solicitați proprietarului comenzii de rezervare să vă ofere acces de proprietar la comanda de rezervare
- **Politică Exchange:** Puteți face schimb de rezervări pentru o altă rezervare de același tip - nu există **pedepse în cazul schimbului** de rezervări. Angajamentul total cu noua rezervare ar trebui să fie mai mare decât suma rambursării schimbate și plățile lunare viitoare (dacă este cazul)
- **Politica de rambursare:** Suma rambursării și plățile viitoare anulate nu pot depăși 50.000 USD într-o fereastră continuă de 12 luni. În prezent **nu percepem nicio taxă pentru rambursări,** dar ar putea fi taxat cu privire la rambursările viitoare

**Excepții:** Posibilitatea de schimb și anulare cu autoservire nu este disponibilă pentru clienții cu Acord Us Government Enterprise

- **Asistența API/PS/ CLI** nu este disponibilă pentru anulare și rambursări cu [autoservre și rambursări pentru rezervări Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Posibilitatea de schimb și anulare cu autoservire nu este disponibilă pentru clienții cu Acord Us Government Enterprise. Sunt acceptate alte tipuri de abonamente pentru guvernul SUA, inclusiv Pay-As-You-Go și CSP

Aflați mai multe: [Cum sunt procesate](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) tranzacțiile de returnare și exchange Aflați mai multe: [Politicile Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) și de rambursare Alte [întrebări: Vizitați documentele instanțelor rezervate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange o instanță rezervată existentă (autoservre)**

Puteți face schimb de rezervări pentru o altă rezervare de același tip. De asemenea, puteți rambursa o rezervare, de până la 50.000 USD pe an, dacă nu mai aveți nevoie de aceasta. Posibilitatea de schimb și anulare cu autoservire nu este disponibilă pentru clienții cu Acord Us Government Enterprise. Sunt acceptate alte tipuri de abonamente pentru guvernul SUA, inclusiv Pay-As-You-Go și CSP. Trebuie să aveți acces la proprietar în Comanda de rezervare pentru a face schimb sau a rambursa o rezervare existentă.

Pașii următori vă vor ghida în procedura de finalizare a tranzacției

1.Conectați-vă la [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervările pe care doriți să le restituiți și faceți clic pe **Exchange** 2.Selectați produsul VM pe care doriți să-l cumpărați și tastați o cantitate. Asigurați-vă că noul total de achiziție este mai mare decât totalul returnat [Determinați dimensiunea corectă înainte de a cumpăra](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Revizuiți și finalizați tranzacția

**Rambursare pentru o instanță rezervată**

Pentru a rambursa o rezervare, accesați Detalii rezervare **și faceți** clic pe **Rambursare**

**Rambursare pro-evaluată:**

**Exemple de prorationare și cerință minimă pentru rambursare și schimb** Exemplu de rezervare din upfront:

- Achiziționați un RI pe termen de un an la prețul de 120 $ la 1 ianuarie
- Pe 7 aprilie, doriți să faceți o rambursare sau să faceți schimb cu această rezervare
- Deoarece rezervarea a fost live timp de 97 de zile, veți primi (1-97/365) * 120 LEI înapoi. (de exemplu, 88,1 LEI). În prezent nu există niciun peisa pentru rambursări
- Dacă schimbul, noua dvs. achiziție ar trebui să fie mai mare de 88,1 LEI
- În prezent nu există rambursare

**Exemplu de rezervare a planului de facturare:**

- Achiziționați un RI pe termen de un an la prețul de 10 $ pe lună
- Pe 7 aprilie, doriți să faceți o rambursare sau să faceți schimb cu această rezervare
- Deoarece ultima plată a fost efectuată cu 7 zile, veți primi (07.01.2031) * 10 LEI înapoi. (de exemplu, 7,74 dolari)
- Plățile viitoare anulate sunt de 80 LEI. În prezent nu există niciun peisa pentru rambursări
- Această anulare va returna 87,74 LEI din limita de rambursare de 50.000 lei
- Dacă schimbul, valoarea totală a achiziției noi ar trebui să fie mai mare de 87,74 lei

**Nu pot vedea factura pentru ultima perioadă de facturare**

Unele motive posibile pentru care este posibil să nu vedeți o factură:

- Aveți o sumă de credit lunară în abonament pe care nu ați depășit-o sau aveți o versiune de încercare gratuită. O factură este generată doar atunci când datorați bani
- Sunt mai puțin de 30 de zile din ziua în care v-ați abonat la Azure
- Factura nu este generată încă. Așteptați până la sfârșitul perioadei de facturare
- Dacă nu fiți administratorul de cont, este posibil ca facturile mai vechi să nu fie disponibile pentru dvs.

**Descărcați factura de pe portalul Azure (.pdf)**

- Selectați-vă abonamentul [din pagina](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Abonamente din portalul [Azure, ca utilizator cu acces la facturi](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selectați **Facturi**
- Faceți **clic pe** Descărcare factură pentru a vizualiza o copie a facturii PDF. Dacă pe acesta **scrie Indisponibil**, consultați De ce nu văd o factură pentru ultima perioadă [de facturare?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Primirea facturii prin e-mail (.pdf)**

- Selectați abonamentul din [pagina Abonamente.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Faceți **clic pe Facturi, apoi** trimiteți factura prin e-mail
- Faceți **clic pe** înscriere și acceptați termenii. Va trebui să optați pentru fiecare abonament pe care îl dețineți

Notă: Dacă nu obțineți un e-mail după ce urmați [pașii,](https://account.windowsazure.com/profile) asigurați-vă că adresa de e-mail este corectă în preferințele de comunicare din profilul dvs.

**Descărcarea datelor de utilizare din portalul Azure**

- Conectați-vă [la Centrul de conturi Azure](https://account.windowsazure.com/Subscriptions) ca administrator de [cont](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Selectați abonamentul pentru care doriți factura și informațiile de utilizare
- Selectați **Istoricul de facturare**
- Selectați **Vedeți inserția** curentă pentru a vedea o estimare a costurilor în momentul când a fost generată estimarea
- Selectați **Descărcați** utilizarea pentru a descărca datele de utilizare zilnică ca fișier CSV. Dacă vedeți două versiuni disponibile, descărcați versiunea 2

Alte întrebări: [Vizitați documentele instanță rezervată](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documente recomandate**

- [Noțiuni de bază despre facturare](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți cum se aplică reducerea pentru Instanța rezervată](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Descărcați sau vizualizați factura Azure și datele de utilizare zilnică](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți cum se aplică reducerea pentru Instanța rezervată](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți utilizarea instanțelor rezervate pentru abonamentul dvs. Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți utilizarea instanțelor rezervate pentru înscrierea dvs. Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Costurile de software Windows nu sunt incluse cu instanțe rezervate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instanțe rezervate în programul furnizor central de soluții cloud pentru parteneri (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)