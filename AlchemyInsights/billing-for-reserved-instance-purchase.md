---
title: Facturarea pentru achiziția instanței rezervate
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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104032"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturarea pentru achiziția instanței rezervate

Achiziția instanței rezervate este debitată prin metoda de plată asociată abonamentului pe care îl selectați în momentul achiziționării. Tipul de abonament trebuie să fie un Contract Enterprise (numărul ofertei: MS-AZR-0017P), Plătiţi pe măsură ce vorbiţi (numărul ofertei: MS-AZR-0003P), Microsoft Customer Agreement sau CSP.

- Pentru un abonament de întreprindere, taxele sunt deduse din soldul angajamentului financiar al înregistrării sau sunt facturate suplimentar.
- Pentru abonamentul Plătiți pe măsură ce vorbiți, plățile sunt facturate prin cardul de credit sau prin metoda de plată prin factură din abonament

**Anularea rezervării**

- **Autoservire:** puteți să anulați sau să schimbați singur o instanță rezervată, utilizând [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervarea și faceți clic pe rambursare sau schimb. Rețineți că trebuie să aveți acces de proprietar la comanda de rezervare pentru a realiza schimbul sau rambursarea. Accesul doar la rezervare nu vă va permite să continuați cu rambursarea sau schimbul. Solicitați-i proprietarului comenzii de rezervare să vă ofere acces de proprietar la comanda de rezervare
- **Politică de schimb:** Puteți să schimbați o rezervare cu o altă rezervare de același tip; nu există **nicio penalizare** pentru schimbul de rezervare. Totalul angajat cu noua rezervare ar trebui să fie mai mare decât suma dintre rambursarea rezervării schimbate și plățile lunare viitoare (dacă este cazul)
- **Politica de rambursare:** suma rambursării și plățile viitoare anulate nu pot depăși 50.000 de USD într-o perioadă rulantă de 12 luni. Momentan **nu percepem nicio taxă de penalizare** pentru rambursări, dar am putea să o percepem pentru rambursări viitoare

**Excepții:** schimbul cu autoservire și capacitatea de anulare nu sunt disponibile pentru clienții US Government Enterprise Agreement

- Asistența **API/PS/CLI** nu este disponibilă pentru anulare și [schimburi cu autoservire ale rambursărilor pentru rezervările Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Schimbul cu autoservire și capacitatea de anulare nu sunt disponibile pentru clienții US Government Enterprise Agreement. Alte tipuri de abonamente pentru Guvernul SUA, inclusiv Plătiţi pe măsură ce vorbiţi și CSP, sunt acceptate

Aflați mai multe: [Cum sunt procesate](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) tranzacțiile de returnare și exchange Aflați mai multe : [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) și politicile de rambursare Alte întrebări: Vizitați [documentele instanțelor rezervate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Schimbați o instanță rezervată existentă (autoservire)**

Puteți să schimbați o rezervare cu o altă rezervare de același tip. De asemenea, puteți să rambursați o rezervare de până la 50.000 de USD anual, dacă nu mai aveți nevoie de aceasta. Schimbul cu autoservire și capacitatea de anulare nu sunt disponibile pentru clienții US Government Enterprise Agreement. Alte tipuri de abonamente pentru Guvernul SUA, inclusiv Plătiţi pe măsură ce vorbiţi și CSP, sunt acceptate. Rețineți că trebuie să aveți acces de proprietar la comanda de rezervare pentru a schimba sau a rambursa o rezervare existentă.

Pașii următori vor oferi orientări cu privire la procedura de finalizare a tranzacției

1.Conectați-vă la [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervările pe care doriți să le rambursați și faceți **clic Exchange** 2.Selectați produsul VM pe care doriți să-l cumpărați și tastați o cantitate. Asigurați-vă că noul total de achiziție este mai mare decât totalul returnat [Determinați dimensiunea corectă înainte de a cumpăra](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Revizuiți și finalizați tranzacția

**Rambursați o instanță rezervată**

Pentru a rambursa o rezervare, accesați **Detalii rezervare** și faceți clic pe **Rambursare**

**Rambursare proporțională:**

**Pro de rambursare și exemple minime de cerințe pentru rambursare și schimb** Exemplu de rezervare din upfront:

- La 1 ianuarie, achiziționați o instanță de rezervare (RI) de un an pentru 120 de USD
- Pe 7 aprilie, doriți să rambursați sau să schimbați această rezervare
- Deoarece rezervarea a fost activă timp de 97 de zile, veți primi înapoi (1-97/365) * 120 de USD. (adică 88,1 USD). În prezent, nu există nicio penalizare pentru rambursări
- Dacă realizați un schimb, noua achiziție ar trebui să fie mai mare de 88,1 USD
- În prezent, nu există nicio penalizare pentru rambursări

**Exemplu de rezervare a planului de tarifare:**

- Achiziționați o instanță de rezervare (RI) de un an pentru 10 USD pe lună
- Pe 7 aprilie, doriți să rambursați sau să schimbați această rezervare
- Deoarece ultima plată a avut loc în urmă cu 7 zile, veți primi înapoi (1-7/31) * 10 USD. (adică 7,74 USD).
- Plățile viitoare anulate sunt de 80 USD. În prezent, nu există nicio penalizare pentru rambursări
- Această anulare va deduce suma de 87,74 USD din limita rambursării de 50.000 de USD
- Dacă realizați un schimb, valoarea totală a noii achiziții ar trebui să fie mai mare de 87,74 USD

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

Alte întrebări:[Consultați documente pentru instanța rezervată](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documente recomandate**

- [Noțiuni de bază despre facturare](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți cum se aplică reducerea pentru Instanța rezervată](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Descărcați sau vizualizați factura Azure și datele de utilizare zilnică](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți cum se aplică reducerea pentru Instanța rezervată](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți utilizarea instanțelor rezervate pentru abonamentul dvs. Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Înțelegeți utilizarea instanțelor rezervate pentru înscrierea dvs. Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows software nu este inclus în instanțele rezervate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instanțe rezervate în programul Partner Central Furnizor de soluții cloud (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)