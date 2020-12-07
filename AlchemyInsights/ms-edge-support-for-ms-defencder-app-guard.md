---
title: Asistența Microsoft Edge pentru Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584013"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Asistența Microsoft Edge pentru Microsoft Defender Application Guard

Proiectat pentru Windows 10 și Microsoft Edge, Guard Application utilizează o abordare de izolare hardware care permite unui utilizator să navigheze pe un site care nu este de încredere din interiorul unui container izolat, Hyper-V-enabled, separat de sistemul de operare gazdă.

Un administrator de întreprindere definește o listă de site-uri web de încredere, resurse cloud și rețele interne. Atunci când un utilizator vizitează un site care nu se află în listă, Microsoft Edge va deschide site-ul în container. Acest lucru înseamnă că, dacă site-ul se dovedește a fi rău intenționat, PC-ul gazdă va rămâne protejat, iar atacatorul nu va accesa datele întreprinderii.

Instalarea extensiilor în container este acceptată de Microsoft Edge Version 81 și poate fi controlată prin intermediul unei politici. Adresa updateURL care se utilizează în politica ExtensionInstallForcelist ar trebui să fie adăugată ca resursă neutră în politicile de izolare a rețelei utilizate de Garda de aplicații.

Pentru mai multe informații, consultați [asistența Microsoft Edge pentru Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
