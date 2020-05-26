---
title: 'Scaner AIP: instalare și configurare'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358105"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scaner AIP: instalare și configurare

**Pentru a instala scanerul AIP, urmați instrucțiunile recomandate:**

1. Dacă faceți upgrade și nu efectuați o instalare curată, asigurați-vă că ați urmat instrucțiunile pentru [upgrade-ul scanerului Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) și pentru clientul unificat de etichetare, consultați [upgrade-ul scanerului Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Verificați dacă respectați toate [cerințele privind paravanele de protecție și setările de infrastructură de rețea](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Asigurați-vă că [politicile sunt setate](https://docs.microsoft.com/azure/information-protection/configure-policy) la etichetare automată sau că aveți o etichetă implicită în politică.
4. Asigurați-vă că tipul de fișier relevant este configurat pentru etichetă/protecție așa este descris în [tipuri de fișiere acceptate de clientul Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). În plus, dacă doriți să modificați comportamentul implicit, urmați aceste instrucțiuni: [Modificarea nivelului implicit de protecție a fișierelor](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verificați că contul de utilizator configurat pentru a executa serviciul de scaner are permisiuni pentru a accesa toate depozitele configurate.
6. Dacă întâmpinați în continuare probleme, exportați jurnalele scanerului și adăugați-le la biletul de asistență.

**Export azure informații protecție scaner jurnalele**

1. Navigați la %localappdata%\Microsoft\MSIP sub contextul utilizatorului care execută serviciul de scanare.
2. Zip tot conținutul sub folderul MSIP.
3. Salvați jurnalele la alegerea locației și atașați-le la solicitarea de serviciu.
4. Puteți utiliza, de asemenea, [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Pentru informații suplimentare, consultați:**
- [Implementarea scanerului Azure Information Protection pentru a clasifica și proteja automat fișierele](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Specificați și utilizați parametrul Simbol pentru Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Executarea unui ciclu de descoperire și vizualizarea rapoartelor pentru scaner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Examinați documentația Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Cerințe pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Descărcați clientul Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
