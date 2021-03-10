---
title: Faceți descoperirea site-ului
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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694560"
---
# <a name="do-site-discovery"></a>Faceți descoperirea site-ului

Dacă organizația utilizează încă aplicații web moștenite și intenționează să utilizeze modul Internet Explorer (pe care o fac majoritatea clienților), ar trebui să efectuați o descoperire suplimentară a site-ului.

**Ați implementat deja o versiune mai veche de Microsoft Edge**

Dacă ați configurat deja lista de site-uri de întreprindere pentru a lucra pentru versiunea moștenită de Microsoft Edge, atunci descoperirea site-ului este aproape gata. Singurul lucru pe care ar trebui să-l faceți este să adăugați site-uri neutre.

Site-urile neutre sunt de obicei site-uri care furnizează sign-on unic (SSO). Dacă accesați un site neutru din Microsoft Edge, atunci doriți să rămâneți în Microsoft Edge pentru a vă autentifica. Dacă accesați un site neutru în modul Internet Explorer, atunci doriți să rămâneți în modul Internet Explorer pentru a vă autentifica.

Identificați orice SSO sau alte site-uri neutre pe care le utilizați și adăugați-le în lista de site-uri de întreprindere.

**Internet Explorer este browserul implicit**

Dacă utilizați acum Internet Explorer, este posibil să nu știți ce site-uri au făcut upgrade la standardele web moderne și care necesită încă Internet Explorer. Veți dori să găsiți și să adăugați aceste site-uri la lista site-ului de întreprindere, astfel încât să puteți utiliza modul Internet Explorer doar pentru acele site-uri.

> [!NOTE]
> [Descoperirea site-ului Enterprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) descoperă site-uri care pot necesita modul Internet Explorer. Poate colecta date pe computerele care execută Windows Internet Explorer 8 prin Internet Explorer 11 în Windows 10, Windows 8,1 sau Windows 7.

**Analizarea datelor**

După ce ați colectat datele de site, vă recomandăm următorul proces în patru pași pentru a analiza datele:
1. Sortați datele după domeniu, apoi după URL.
2. Definiți limitele unei aplicații pentru a configura modul Internet Explorer. Doriți să includeți toate site-urile și controalele web care definesc aplicația, dar nu doriți să includeți site-uri și controale suplimentare. Unele site-uri pot fi la fel de simple ca *https://contoso.com/app1* în timp ce alte persoane vă pot solicita să definiți mai multe site-uri și pagini.
3. Testați aplicația pentru a verifica dacă nu funcționează în mod nativ. Multe site-uri vor oferi conținut modern atunci când detectează un browser modern și oferă doar conținut moștenit atunci când detectează Internet Explorer.
4. Adăugați aplicația la lista de site-uri de întreprindere dacă nu reușește testarea.

> [!NOTE]
> Ca o practică optimă, grupați toate site-urile care cuprind o aplicație. În acest fel, atunci când faceți upgrade unei aplicații, este mai ușor să eliminați întregul site din modul Internet Explorer și să începeți să utilizați un browser modern pentru acea aplicație.

După ce ați terminat cu descoperirea site-ului și ați analizat datele, sunteți gata să începeți să vă uitați la strategia de canal.

