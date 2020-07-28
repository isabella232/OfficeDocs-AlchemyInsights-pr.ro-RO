---
title: Mai multe obiecte au aceeași adresă de e-mail ca și identitatea
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439713"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Mai multe obiecte au aceeași adresă de e-mail ca și identitatea

**Mai multe obiecte**

Unul dintre motivele comune ale acestei erori este că nu se poate distribui corect o solicitare Outlook Web Access într-o prezență a mai multor obiecte care au aceeași adresă de e-mail ca și identitatea. Pentru a găsi aceste obiecte, executați următoarele comenzi:

· Obțineți-destinatar<email address>

· Obțineți-utilizator<email address>

· Utilizator-get <email address> -SoftDeletedUser

· Contact-contact<email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxNumai

Pentru a rezolva problema, eliminați mai multe obiecte cu aceeași identitate de e-mail și asigurați-vă că există un singur obiect cu identitatea de e-mail specifică și că tipul său de destinatar este UserMailbox.

**Aceeași adresă este utilizată pentru cutiile poștale de afaceri și de consum**

O altă cauză este atunci când aceeași adresă este utilizată pentru cutiile poștale de afaceri și de consum. În acest caz, utilizatorul trebuie să schimbe alias lor de consum primar până când Cafe acceptă acest scenariu. Aceasta este o eroare permanentă care nu dispare fără intervenție.

Pentru detalii, consultați [Modificarea adresei de e-mail sau a numărului de telefon pentru contul Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).