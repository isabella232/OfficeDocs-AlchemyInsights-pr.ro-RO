---
title: Nu se poate activa Office
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
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327858"
---
# <a name="unable-to-activate-office"></a>Nu se poate activa Office

**Notă:** Dacă utilizați o versiune mai veche de Windows (de exemplu, Windows 7), asigurați-vă că TLS 1.2 este activat ca implicit. Pentru mai multe informații, consultați Actualizarea pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)protocoale sigure implicite în WinHTTP în Windows .

- Verificați dacă abonamentul dvs. a expirat.
- Asigurați-vă că aveți un abonament care permite licențe client, cum ar fi Office 365 Business sau Business Premium, și [ asigurați-vă că utilizatorul are atribuită o licență](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Asigurați-vă că utilizatorul se conectează la Office cu același cont căruia i s-a atribuit licența.
- Verificați [pagina de stare a serviciilor Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) pentru a vedea dacă există probleme cunoscute cu serviciul.
- Verificați firewallul, programul antivirus și setările de proxy pentru a confirma că acestea nu blochează accesul aplicațiilor Microsoft 365 la internet. Consultați [Adrese URL și intervale de adrese IP Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Adrese URL și intervale de adrese IP Office 365").

**Sfat** Pe computerele Windows putem diagnostica și remedia automat pentru dvs. mai multe probleme comune de conectare la Office. Descărcați și rulați **[Asistentul pentru recuperare și asistență pentru Office 365](https://aka.ms/SaRA-OfficeSignInScenario)** pentru a utiliza instrumentul nostru automatizat.

Utilizați următoarele acțiuni de depanare:

- Deschideți o aplicație Office și [deconectați-vă](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) din conturile de utilizator existente. [Eliminați](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) și [reatribuiți](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licența Office, apoi [conectați-vă la Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) utilizând contul de utilizator afectat.
- Rulați [Depanatorul de activare](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Resetați starea de activare Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Resetați starea de activare Office")
- [Efectuarea unei reparări Online a Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Pentru soluții de depanare suplimentare, consultați:  

- [Erorile de activare și „Produs nelicențiat” în Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Eroarea „Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu” atunci când activați Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)