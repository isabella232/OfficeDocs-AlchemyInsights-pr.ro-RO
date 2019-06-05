---
title: A crea şi de a folosi o cutie poştală partajată
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717358"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Depanaţi problema - utilizatorul nu a fost găsit în Director

<p>În cazul în care utilizatorii primesc mesaj de eroare <strong> &ldquo; &hellip;utilizator poate&rsquo;t se află în directorul. Vă rugăm să încercaţi din nou&hellip; </strong> în cazul în care tipul de problemă este <strong> &ldquo;utilizator nu în director.&rdquo;</strong>, poate fi terminat următorii paşi pentru a depana problema.</p> <ol> <li>Asigura contului care a acceptat invitaţia e-mail este acelaşi cont, care este folosit să semneze mai târziu. Asiguraţi-vă că utilizatorul este folosind acelaşi cont pentru a accepta invita şi conectaţi-vă site-ul. <br /><br />Pentru mai multe informaţii, a se vedea <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">cum să gestionaţi pseudonime pentru contul Microsoft</a> pentru a gestiona logare Office 365. <br /><br /></li> <li>Navigaţi la fiecare site în care utilizatorul primeşte eroare. <br /><br />un. Adauga <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (în dublu-ghilimele) la sfârşitul URL-ul site-ului. <br /><br />Exemplu: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Selectaţi utilizator din listă. <br /><br />c. Faceţi clic pe <strong>Eliminare permisiuni utilizator din panglică</strong>. <br /><br />d. Adauga înapoi utilizatorului şi retrimiteţi a invita pentru utilizator.</li> </ol>

