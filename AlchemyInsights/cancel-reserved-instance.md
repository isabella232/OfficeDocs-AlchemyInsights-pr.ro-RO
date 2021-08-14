---
title: Anularea rezervării
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931245"
---
# <a name="cancelling-reservation"></a>Anularea rezervării

- **Autoservire:** puteți să anulați sau să schimbați singur o instanță rezervată, utilizând [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervarea și faceți clic pe rambursare sau schimb. Rețineți că trebuie să aveți acces de proprietar la comanda de rezervare pentru a realiza schimbul sau rambursarea. Accesul doar la rezervare nu vă va permite să continuați cu rambursarea sau schimbul. Solicitați-i proprietarului comenzii de rezervare să vă ofere acces de proprietar la comanda de rezervare
- **Politică de schimb:** Puteți să schimbați o rezervare cu o altă rezervare de același tip; nu există **nicio penalizare** pentru schimbul de rezervare. Totalul angajat cu noua rezervare ar trebui să fie mai mare decât suma dintre rambursarea rezervării schimbate și plățile lunare viitoare (dacă este cazul)
- **Politica de rambursare:** suma rambursării și plățile viitoare anulate nu pot depăși 50.000 de USD într-o perioadă rulantă de 12 luni. Momentan **nu percepem nicio taxă de penalizare** pentru rambursări, dar am putea să o percepem pentru rambursări viitoare  
    **Excepții:** schimbul cu autoservire și capacitatea de anulare nu sunt disponibile pentru clienții US Government Enterprise Agreement
- Asistența **API/PS/CLI** nu este disponibilă pentru anulare și [schimburi cu autoservire ale rambursărilor pentru rezervările Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Schimbul cu autoservire și capacitatea de anulare nu sunt disponibile pentru clienții US Government Enterprise Agreement. Alte tipuri de abonamente pentru Guvernul SUA, inclusiv Plătiţi pe măsură ce vorbiţi și CSP, sunt acceptate

Aflați mai multe: [Cum sunt procesate tranzacțiile de schimb și de restituire](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Aflați mai multe: [Politicile de schimb și de rambursare](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Alte întrebări:[Consultați documente pentru instanța rezervată](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Schimbați o instanță rezervată existentă (autoservire)**

Puteți să schimbați o rezervare cu o altă rezervare de același tip. De asemenea, puteți să rambursați o rezervare de până la 50.000 de USD anual, dacă nu mai aveți nevoie de aceasta. Schimbul cu autoservire și capacitatea de anulare nu sunt disponibile pentru clienții US Government Enterprise Agreement. Alte tipuri de abonamente pentru Guvernul SUA, inclusiv Plătiţi pe măsură ce vorbiţi și CSP, sunt acceptate. Rețineți că trebuie să aveți acces de proprietar la comanda de rezervare pentru a schimba sau a rambursa o rezervare existentă.

Pașii următori vor oferi orientări cu privire la procedura de finalizare a tranzacției

1. Conectați-vă la [portalul Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Selectați rezervările pe care doriți să le rambursați și faceți clic pe **Schimb**
2. Selectați produsul VM pe care doriți să-l achiziționați și tastați o cantitate. Asigurați-vă că noul total al achiziției este mai mare decât totalul restituit [Stabiliți dimensiunea corectă înainte de achiziționare](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Revizuiți și finalizați tranzacția

**Rambursați o instanță rezervată**

Pentru a rambursa o rezervare, accesați **Detalii rezervare** și faceți clic pe **Rambursare**

**Rambursare proporțională:**

**Exemple de tarifare fracționară și cerințe minime pentru rambursare și schimb**  
Exemplu de rezervare în prealabil:

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

**Documente recomandate**

- [Cum sunt procesate tranzacțiile de schimb și de rambursare](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Politicile de schimb și de rambursare](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)