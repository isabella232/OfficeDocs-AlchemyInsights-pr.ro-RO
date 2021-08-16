---
title: Intune Exchange conector local
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013976"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange conector local

Pentru detalii despre configurarea conectorului între Intune și Exchange care este găzduit local, consultați documentația următoare:

[Configurarea conectorului Detune Exchange local în Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Întrebări frecvente:**

Î: Văd o eroare, cum ar fi "The Exchange Connector version is not supported" (Versiunea Exchange Connector nu este acceptată) atunci când încerc să configurați conectorul Exchange conector. Care ar putea fi cauza?

A: Contul pe care îl utilizați este licențiat în mod corespunzător - trebuie să aibă o licență Intune activă

Î: Este posibil să aveți mai mulți Exchange conectori?

A: Puteți configura un singur conector de Exchange pentru fiecare entitate găzduită Intune Exchange organizație. Conectorul poate fi instalat pe un singur server într-o organizație de schimb de servere multiple.

De asemenea, nu puteți configura conectori atât pentru Exchange local, cât Exchange Online configurați în aceeași entitate găzduită.

Î: Conectorul poate utiliza o matrice CAS ca conexiune la Exchange?

A: Specificarea unei matrice CAS nu este o configurație acceptată în configurarea conectorului. Ar trebui să fie specificat un singur server și ar trebui să fie codat hardcoded în fișierul de configurare al conectorului, care poate fi găsit în

date program\microsoft\microsoft Intune local Exchange conector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Găsiți următoarea intrare ```<ExchangeWebServiceURL />``` și înlocuiți adresa URL cu serverul Exchange.

**Exemplu:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consultați documentația următoare pentru depanare suplimentară: [Depanarea conectorului local Intun Exchange e](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Activarea înregistrării detaliate în jurnal pentru Exchange conector**

1. Deschideți fișierul de Exchange de configurare a urmăririi conectorului pentru editare.  
Fișierul se află la : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exemplu:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Găsiți TraceSourceLine cu următoarea cheie: OnPremisesExchangeConnectorService  
  
3. Modificați valoarea nodului SourceLevel din Information ActivityTracing (implicit) la Verbose ActivityTracing  

**Exemplu:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Reporniți serviciul Microsoft Intune Exchange service  
5. Sincronizare completă în Portalul Intune până când se termină, apoi schimbați XML din nou la "Information ActivityTracing" și reporniți serviciul Microsoft Intune Exchange SERVICE.  
6. Locația jurnalelor este: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`