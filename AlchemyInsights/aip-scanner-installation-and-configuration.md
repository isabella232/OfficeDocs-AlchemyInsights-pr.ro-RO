---
title: 'Scaner AIP: instalare și configurare'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934269"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scaner AIP: instalare și configurare

**Pentru a instala scanerul AIP, urmați instrucțiunile recomandate:**

1. Dacă faceți upgrade și nu efectuați o instalare curată, asigurați-vă că ați urmat instrucțiunile pentru upgrade-ul scanerului [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) și pentru clientul de etichetare unificată, consultați Upgrade-ul scanerului Azure Information [Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Verificați dacă respectați toate cerințele de [setări pentru firewalluri și infrastructură de rețea.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Asigurați-vă [că politicile dvs.](https://docs.microsoft.com/azure/information-protection/configure-policy) sunt setate la etichetare automată sau au o etichetă implicită în politică.
4. Asigurați-vă că tipul de fișier relevant este configurat pentru etichetă/protecție, așa cum este descris în Tipurile de fișier acceptate [de clientul Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) În plus, dacă doriți să modificați comportamentul implicit, urmați aceste instrucțiuni: [Modificarea nivelului de protecție implicit pentru fișiere.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Verificați dacă acel cont de utilizator configurat pentru a rula serviciul de scaner are permisiunea de a accesa toate depozitele configurate.
6. Dacă încă mai experimentați probleme, exportați jurnalele de scaner și adăugați-le în tichetul de asistență.

**Exportul jurnalelor de scaner de protecție a informațiilor Azure**

1. Navigați la %localappdata%\Microsoft\MSIP sub contextul de utilizator care rulează serviciul de scaner.
2. Arhivați tot conținutul din folderul MSIP.
3. Salvați jurnalele la alegerea locației și atașați-le la solicitarea de serviciu.
4. De asemenea, puteți [utiliza Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Pentru informații suplimentare, consultați:**
- [Implementarea scanerului Azure Information Protection pentru a clasifica și a proteja automat fișierele](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Specificarea și utilizarea parametrului Token pentru Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Rulați un ciclu de descoperire și vizualizați rapoarte pentru scaner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Revizuiți documentația Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Cerințe pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Descărcați clientul Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
