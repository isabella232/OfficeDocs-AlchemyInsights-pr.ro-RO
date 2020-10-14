---
title: Implementarea aplicațiilor Win32 Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461877"
---
# <a name="intune-win32-app-deployment"></a>Implementarea aplicațiilor Win32 Intune

Microsoft Intune permite aplicațiilor Win32, inclusiv, dar fără a se limita la MSI și. EXE va fi implementat pe dispozitivele Windows 10. Mecanismul de implementare utilizat necesită ca extensia de gestionare Intune (IME) să fie prezentă pe dispozitivul țintă. IME va fi instalat automat ca urmare a țintirei unui script PowerShell sau a unei implementări de aplicații Win32 la un utilizator/dispozitiv.

Există, de asemenea, un set de cerințe preliminare care trebuie îndeplinite pentru a implementa aplicații Win32 care includ:

- Platforme acceptate: Windows 10 versiunea 1607 sau o versiune mai recentă (versiunile Enterprise, Pro și Education).
- Arhitectură acceptată: x86 și x64.
- Gestionarea dispozitivelor: Dan s-a alăturat și s-a înscris automat (inclusiv domeniul hibrid asociat și s-a înscris automat în Politica de grup).
- Format pachet de aplicații:. fișier **intunewin**  pregătit de [instrumentul Microsoft Win32 Content Prep](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Limite
    - Dimensiunea maximă: 8GB.
    - Arhitectură neacceptată: ARMs.

Revizuiți documentul "[adăugarea, atribuirea și monitorizarea unei aplicații Win32 în Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" pentru informații legate de acești pași.

Detalii despre depanarea implementării aplicațiilor pe Windows, inclusiv aplicațiile Win32 pot fi revizuite în următoarele documente

- [Depanarea problemelor de instalare a aplicațiilor](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Depanarea aplicațiilor Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)