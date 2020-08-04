---
title: Utilizarea TeamViewer pentru administrarea de la distanță a dispozitivelor Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555246"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Utilizarea TeamViewer pentru administrarea de la distanță a dispozitivelor Intune

Dispozitivele gestionate de Intune pot fi administrate de la distanță utilizând [TeamViewer](https://www.teamviewer.com/).

Pentru a administra Intune utilizând TeamViewer, utilizați acești pași: 

Începeți prin a obține acreditări de la TeamViewer pentru a configura Conectorul TeamViewer pe Intune. Acest lucru permite administratorului să introducă acreditări în interfața de utilizator a conectorului TeamViewer sub Dispozitive, o operațiune o singură dată pentru a stabili legătura dintre Intune și serviciul TeamViewer.

**Partea 1: Începerea unei sesiuni cu un dispozitiv la distanță**

1. Sub **Toate dispozitivele**, selectați dispozitivul cu care doriți să începeți o sesiune la distanță.
2. De la **... Mai mult**, selectați **Sesiune nouă de asistență la distanță**.
3. Selectați **Da** pentru a confirma că doriți să stabiliți o sesiune la distanță.
    După ce solicitarea "Inițierea unei noi sesiuni la distanță" este recunoscută de serviciul TeamViewer, veți vedea o opțiune pentru **a porni asistența la distanță** sub detaliile panoului Prezentare generală (sau, Essentials) pentru dispozitiv. Selectați **Vedeți mai multe** pentru a extinde panoul și a afișa starea Asistență la distanță.
4. Selectați **Pornire sesiune la distanță** pentru a iniția sesiunea pe partea de administrator.
5. Alegeți să descărcați binarul TeamViewer (Windows) și selectați **Executare**.<br/>
    **Notă** Puteți ignora orice pagină de browser web deschisă site-ului Web TeamViewer.

6. Confirmați solicitarea ca aplicația TeamViewer să efectueze modificări pe dispozitiv (numai Windows).
7. Aplicația TeamViewer pornește și include codul de sesiune pentru a autentifica conexiunea cu dispozitivul la distanță.

**Partea 2: Pe dispozitivul vizat pentru o sesiune la distanță**

1. Deschideți portalul companiei Intune.
2. Căutați un semnalizator de notificare: "Administratorul IT solicită controlul acestui dispozitiv pentru o sesiune de asistență la distanță" și selectați notificarea.
3. Alegeți să descărcați aplicația TeamViewer sau să confirmați descărcarea aplicației TeamViewer din magazinul de aplicații și selectați **Executare**.
    **Notă** Puteți ignora orice pagină de browser web deschisă site-ului Web TeamViewer.

4. Confirmați solicitarea ca aplicația TeamViewer să efectueze modificări pe dispozitiv (numai Windows).
5. Aplicația TeamViewer pornește și include codul de sesiune pentru a autentifica conexiunea cu dispozitivul la distanță.
6. Un pop-up întreabă dacă doriți să permiteți începerea sesiunii.

**Notă** Codurile de sesiune generate de serviciul TeamViewer sunt utilizate o singură dată. Dacă pierdeți conexiunea, trebuie:

1. Închideți instanța aplicației TeamViewer pe dispozitivul la distanță și pe aplicația de lucru de administrare.
2. Închideți portalul companiei pe dispozitivul la distanță.
3. Inițiați o nouă "Sesiune nouă de asistență la distanță" din portalul de administrare.
4. Redeschideți portalul companiei pe dispozitivul la distanță pentru a primi noua notificare.
5. Descărcați și deschideți aplicația TeamViewer atât pe dispozitivul la distanță, cât și pe aplicația de lucru de administrare, ca și până acum.