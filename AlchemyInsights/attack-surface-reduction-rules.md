---
title: Regulile de reducere a suprafeței de atac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676440"
---
# <a name="attack-surface-reduction-rules"></a>Regulile de reducere a suprafeței de atac

Excluderea fișierelor sau folderelor poate reduce grav protecția oferită de regulile de reducere a suprafeței de atac. Fișierele care ar fi fost blocate de o regulă au permisiunea de a rula și nu este înregistrat niciun raport sau eveniment. Excluderea se aplică tuturor regulilor care permit excluderi.

Excluderile ASR utilizează aceeași sintaxă ca Antivirus Microsoft Defender excluderile. Pentru detalii, consultați [Configurarea și validarea excluderilor pentru Antivirus Microsoft Defender scanare.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Pentru a evita problemele, [revizuiți Greșelile comune de evitat atunci când definiți excluderi.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Nu toate regulile ASR acceptă excluderile. Pentru a valida dacă regula dvs. acceptă excluderi, consultați tabelul Regulile de [reducere a suprafeței de atac.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Regulile de reducere a suprafeței de atac

Suprafața de atac a organizației dvs. include toate locurile unde un atacant ar putea compromite dispozitivele sau rețelele organizației. Reducerea suprafeței de atac înseamnă protejarea dispozitivelor organizației și a rețelei, ceea ce lasă atacurile cu mai puține modalități de a efectua atacuri. Configurarea regulilor de reducere a suprafeței de atac în Microsoft Defender pentru punctul final vă poate ajuta.

Pentru mai multe informații, consultați:

- [Mapare GUID pentru regula ASR pentru nume](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Cerințe de reguli ASR:
    - [Windows 10 Pro, versiunea 1709 sau o versiune mai recentă](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versiunea 1709 sau o versiune mai recentă](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versiunea 1803 (Canalul semi-anual) sau o versiune mai recentă](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identificați excluderea corectă de aplicat

1. Căutați eventID 1121 sau 1122 în jurnalul Microsoft-Windows-Windows Defender/operațional.

1. Evaluați scenariul și contextul blocului și confirmați că acest scenariu trebuie deblocat.

1. Citiți valoarea Cale din detaliile evenimentului, care este valoarea care definește excluderea.
    - Faceți excluderea cât mai strictă posibil.
    - Aplicați un wildcard acolo unde este necesar (de exemplu, înlocuiți variabila utilizator).

1. Aplicați excluderea în funcție de nevoile dvs. de implementare. Pentru detalii, consultați Particularizarea [regulilor de reducere a suprafeței de atac.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Excluderea nu este onorată

1. Determinați dacă regula acceptă excluderi. Pentru detalii, consultați Regulile [de reducere a suprafeței de atac.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Revizuiți excluderile aplicate și verificați cu datele evenimentului dacă există metacaractere tastare sau interpretate greșit. Pentru mai multe informații, consultați [Tipuri de excluderi acceptate](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. dacă impactul regulii este prea mare, luați în considerare mutarea regulii (înapoi) în Modul auditare pentru a efectua validări suplimentare. Pentru detalii, consultați [Testarea modului în care funcționează caracteristicile Microsoft Defender pentru puncte finale în modul de auditare.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Colectați date de asistență pentru a deschide un caz de asistență utilizând această comandă:
    
   ** MDEClientAnalyzer.cmd -v**

    Pentru mai multe informații, [consultați Probleme cu mașinile de bord la Microsoft Defender pentru puncte finale.](issues-with-onboarding-machines.md)
