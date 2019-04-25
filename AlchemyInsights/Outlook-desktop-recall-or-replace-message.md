---
title: Outlook amintesc Desktop sau înlocuiţi un mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389758"
---
# <a name="recall-or-replace-an-email-message"></a>Amintesc sau să înlocuiască un mesaj de e-mail

- Ca administrator, puteţi **amintesc mesaje în numele utilizatorilor folosind PowerShell**. Nu pot aminti mesaje de la centrul de administrare.
- Puteţi **doar amintesc mesajele care sunt trimise la oameni în cadrul organizaţiei**. Dacă mesajul a fost trimis la o adresă de Gmail, de exemplu, tu nu pot aminti ea.
- Puteţi **doar amintesc mesajele trimise din Outlook 2016 pe PC-ul**. Dacă un utilizator trimite un mesaj cu ajutorul Outlook pentru Mac sau Outlook de pe web, tu nu-l amintesc.

Să-mi amintesc sau să înlocuiască un mesaj de e-mail:

1. În panoul de foldere pe partea stângă a ferestrei Outlook, selectaţi folderul Elemente trimise.
1. Faceţi dublu clic pe mesajul pe care doriţi să se amintească pentru a o deschide.
1. Selectaţi fila **mesaj** şi selectaţi **Acţiuni** > **Amintesc acest mesaj**.
1. Selectaţi **ştergeţi copiilor necitite ale acestui mesaj** sau **ştergeţi copiilor necitite și înlocuirea cu un mesaj nou**, şi apoi selectaţi **OK**.
1. Dacă sunteţi trimite un mesaj de inlocuire, compune mesajul şi selectaţi **trimite**.
1. Succesul sau eşecul de un recall de mesaj depinde de setările de destinatar în Outlook. Pentru câţiva paşi pentru a verifica pe recall, a se vedea [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Caută şi ştergeţi mesajele de e-mail în cadrul organizaţiei

- Dacă nu sunteţi un administrator global, contul trebuie să fie adăugat rolul de Manager eDiscovery sau rol de gestionare conformitate Search pentru a căuta mesajele. Pentru a ºterge mesaje, veţi avea nevoie să se alăture grupului de roluri Gestionare organizaţie sau rol de gestionare căutare și Golire. Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate şi de conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Creaţi un conţinut de căutare](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul pentru a şterge.
- [Conecta la securitatea şi conformitatea centrul PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Dacă utilizaţi autentificarea multi-factor, consultaţi [Conectare la Office 365 securitatea şi conformitatea centrul PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).