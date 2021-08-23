---
title: Setarea Outlook etichetă implicită nu este aplicată
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455089"
---
# <a name="default-outlook-label-setting-not-applied"></a>Setarea Outlook etichetă implicită nu este aplicată

Dacă setările implicite de etichetă Outlook nu se aplică corect și se aplică o altă etichetă sau nu se aplică nicio etichetă, este posibil să vă confruntați cu o problemă cunoscută (MC277818) și să faceți oricare dintre aceste 2 opțiuni pentru a rezolva problema:

**Opțiunea 1:**

1. Accesați Centrul de Microsoft 365 conformitate > **Solutions**  >  **Information Protection.**
1. Selectați **Politici de** etichete și selectați politica de etichete pe care trebuie să o editați (setarea **OutlookDefaultlabel** nu este setată corect în politica de etichete respectivă. Rulați **Get-labelpolicy pentru** a vizualiza această setare), apoi selectați **Edit policy**.
1. Selectați Următorul până când vedeți setarea Aplicați această etichetă implicită  la mesajele de e-mail **,** care este disponibilă dacă selectați Solicitați utilizatorilor să aplice o etichetă în mesajele de e-mail și documentele sale din caseta de **dialog** Setări politică. 
1. În caseta de dialog **Aplicați o etichetă implicită** la documente, **alegeți** Fără din lista verticală.
1. Selectați **Următorul** și **Remitere pentru** a salva setările etichetei.

**Opțiunea 2:**

În [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Centrul de securitate și conformitate, utilizați commandletul Set-LabelPolicy pentru a modifica **outlookDefaultlabel** la **Fără** pe {OutlookDefaultLabel="None"}.

Rulare: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Pentru mai multe informații despre etichetele implicite pentru Outlook etichete, [consultați Setarea unei etichete implicite diferite pentru Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).