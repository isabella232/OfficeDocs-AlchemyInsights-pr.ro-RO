---
title: Descoperirea site-ului
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030770"
---
# <a name="do-site-discovery"></a>Descoperirea site-ului

Dacă organizația dvs. utilizează în continuare aplicații web moștenite și planuri pentru a utiliza modul Internet Explorer (lucru pe care-l fac majoritatea clienților), ar trebui să faceți câteva descoperiri suplimentare de site-uri.

**Ați implementat deja o versiune mai veche de Microsoft Edge**

Dacă ați configurat deja Lista de site-uri de întreprindere să lucreze pentru versiunea moștenit de Microsoft Edge, descoperirea site-ului este aproape gata. Un lucru pe care poate fi necesar să-l faceți este să adăugați site-uri neutre.

Site-urile neutre sunt de obicei site-uri care oferă sign-on unic (SSO). Dacă vă întoarceți la un site neutru Microsoft Edge, atunci doriți să rămâneți în Microsoft Edge să vă autentificați. Dacă accesați un site neutru din modul Internet Explorer, atunci doriți să rămâneți în modul Internet Explorer pentru autentificare.

Identificați orice SSO sau orice alte site-uri neutre pe care le utilizați și adăugați-le în Lista de site-uri de întreprindere.

**Internet Explorer este browserul dvs. implicit**

Dacă utilizați doar Internet Explorer acum, este posibil să nu știți ce site-uri au făcut upgrade la standardele web moderne și care necesită totuși Internet Explorer. Veți dori să găsiți și să adăugați aceste site-uri la Lista de site-uri de întreprindere, astfel încât să puteți utiliza modul Internet Explorer doar pentru acele site-uri.

> [!NOTE]
> [Descoperire site-uri de](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) întreprindere descoperă site-urile care pot avea nevoie de modul Internet Explorer. Aceasta poate colecta date de pe computere care rulează Windows Internet Explorer 8 prin Internet Explorer 11 pe Windows 10, Windows 8.1 sau Windows 7.

**Analiza datelor**

După ce ați colectat datele de site, vă recomandăm următorul proces în patru etape pentru a analiza datele:
1. Sortați datele după domeniu, apoi după URL.
2. Definiți limitele unei aplicații de configurat pentru modul Internet Explorer. Doriți să includeți toate site-urile și controalele web care definesc aplicația, dar nu doriți să includeți site-uri și controale suplimentare. Unele site-uri pot fi la fel de simple *https://contoso.com/app1* precum altele vă pot solicita să definiți mai multe site-uri și pagini.
3. Testați aplicația pentru a verifica dacă nu funcționează în mod nativ. Multe site-uri vor oferi conținut modern atunci când detectează un browser modern și oferă conținut moștenit doar atunci când detectează Internet Explorer.
4. Adăugați aplicația la Lista de site-uri de întreprindere dacă nu trece de testare.

> [!NOTE]
> Ca exemplu de bună practică, grupți toate site-urile care includ o aplicație. Astfel, atunci când faceți upgrade unei aplicații, este mai simplu să eliminați întregul site din modul Internet Explorer și să începeți să utilizați un browser modern pentru acea aplicație.

După ce ați terminat cu descoperirea site-ului și ați analizat datele, sunteți gata să începeți să analizați strategia de canal.

