---
title: Amintesc sau să înlocuiască un mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096598"
---
# <a name="recall-or-replace-an-email-message"></a>Amintesc sau să înlocuiască un mesaj de e-mail

- Puteţi **doar amintesc mesajele care sunt trimise la oameni în cadrul organizaţiei**. Dacă mesajul a fost trimis la o adresă de Gmail, de exemplu, tu nu pot aminti ea.
- Puteţi **doar amintesc mesajele trimise din Outlook 2016 pentru PC**. Dacă un utilizator trimite un mesaj cu ajutorul Outlook pentru Mac sau Outlook de pe web, tu nu-l amintesc.
- Dacă sunteţi un admin, puteţi **amintesc mesaje în numele utilizatorilor folosind PowerShell**. Nu pot aminti mesaje de la centrul de administrare. Defilaţi în jos la "Caută şi şterge mesajele de e-mail în organizaţia" pentru mai multe informaţii.

***Amintesc sau să înlocuiască un mesaj de e-mail pe care aţi trimis***
1. În panoul de foldere pe partea stângă a ferestrei Outlook, selectaţi folderul Elemente trimise.
2. Deschideţi mesajul pe care doriţi să-mi amintesc. Trebuie să faceţi dublu clic pentru a deschide mesajul. Selectarea mesajului, astfel încât aceasta apare în panoul de citire vă va permite să amintesc mesajul.
3. Din fila mesaj, selectaţi **acţiunile** > **Amintesc acest mesaj**.
4. Alegeţi **ştergeţi copiilor necitite ale acestui mesaj** sau **ştergeţi copiilor necitite și înlocuirea cu un mesaj nou**, apoi selectaţi **OK**.
5. Dacă sunteţi trimite un mesaj de inlocuire, compune mesajul, apoi selectați **trimite**.
6. Succesul sau eşecul de un recall de mesaj depinde de setările de destinatari în Outlook. 

Pentru mai multe informaţii, inclusiv cum să verificaţi pe recall, [Recall](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)sau înlocuiţi un mesaj de e-mail pe care aţi trimis.

***Căutarea şi ştergeţi mesajele de e-mail în cadrul organizaţiei*** Pentru a căuta şi ştergeţi mesajele de e-mail în cadrul organizaţiei, este mai uşor, dacă sunteţi un admin la nivel mondial. Dacă nu sunteţi un administrator global, contul trebuie adăugat la grupul de roluri de Manager eDiscovery, sau la rolul de gestionare conformitatea căutaţi. Pentru a ºterge mesaje, veţi avea nevoie să se alăture grupului de roluri Gestionare organizaţie sau rol de gestionare căutare și Golire. Permisiunile pentru aceste roluri sunt atribuite în [Centrul de conformitatea securitate &](https://protection.office.com/).

1. [Creaţi un conţinut de căutare](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) pentru a găsi mesajul pentru a şterge.
2. [Conecta la securitate & respectarea centrul PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Dacă utilizaţi Mae, consultaţi [Conectare la Office 365 securitate & respectarea centrul PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 