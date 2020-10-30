---
title: Anularea rezervării
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807992"
---
# <a name="cancelling-reservation"></a>Anularea rezervării

- **Cu** autoservire: Puteți să anulați sau să schimbați singur o instanță rezervată utilizând [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervarea și faceți clic pe rambursare sau pe Exchange. Rețineți că trebuie să aveți acces proprietar în ordinea rezervării, pentru a face schimb sau a rambursa. Accesul la rezervare nu vă va permite să continuați cu rambursarea sau schimbul. Solicitați proprietarului comenzii de rezervare să vă ofere accesul proprietarului la comanda de rezervare
- **Politica Exchange:** Puteți face schimb de rezervări pentru o altă rezervare de același tip – nu există **penalități** la schimbul de rezervări. Angajamentul total al rezervării noi ar trebui să fie mai mare decât suma rambursată a rezervării și a plăților lunare viitoare (dacă este cazul)
- **Politica de rambursare:** Suma restituirilor și plățile viitoare anulate nu pot depăși $50.000 USD într-o fereastră rulantă de 12 luni. **În prezent nu percepem nicio sancțiune** pentru rambursări, dar o putem percepe pentru rambursări viitoare  
    **Excepții:** Capacitățile Exchange și anulare cu autoservire nu sunt disponibile pentru clienții din acordul de întreprindere guvernamentală din S.U.A.
- Asistența **API/PS/CLI** nu este disponibilă pentru anularea și rambursarea [schimburilor și restituirilor cu autoservire pentru rezervări Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Capacitățile Exchange și anulare cu autoservire nu sunt disponibile pentru clienții din acordul de întreprindere guvernamentală din SUA. Alte tipuri de abonamente pentru instituții guvernamentale din SUA, inclusiv plățile în timp și CSP sunt acceptate

Aflați mai multe: [cum sunt prelucrate tranzacțiile de returnare și Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Aflați mai multe: [politicile pentru Exchange și rambursare](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Alte întrebări: [accesați documentele de instanță rezervate](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Schimbul unei instanțe rezervate existente (cu autoservire)**

Puteți face schimb de rezervări pentru o altă rezervare de același tip. De asemenea, puteți să returnați o rezervare, de până la $50.000 USD pe an, dacă nu mai aveți nevoie de el. Capacitățile Exchange și anulare cu autoservire nu sunt disponibile pentru clienții din acordul de întreprindere guvernamentală din SUA. Alte tipuri de abonamente pentru guvern din SUA, inclusiv plățile în timp și CSP, sunt acceptate. Trebuie să aveți acces proprietar în ordinea rezervării pentru a face schimb de taxe sau pentru a rambursa o rezervare existentă.

Următorii pași vor ghida procedura de terminare a tranzacției

1. Conectați-vă la [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervările pe care doriți să le rambursați și faceți clic pe **Exchange**
2. Selectați produsul VM pe care doriți să-l achiziționați și tastați o cantitate. Asigurați-vă că noul total de achiziție este mai mare decât totalul de returnare [determină dimensiunea potrivită înainte de a cumpăra](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Revizuirea și finalizarea tranzacției

**Rambursarea unei instanțe rezervate**

Pentru a rambursa o rezervare, accesați **detaliile rezervării** și faceți clic pe **rambursare**

**Rambursare pro-nominală:**

**Exemple Pro-rație și cerințe minime pentru rambursare și Exchange**  
Exemplu de rezervare în avans:

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

**Documente recomandate**

- [Cum sunt prelucrate tranzacțiile de returnare și Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Politici de schimb și rambursare](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)