---
title: Conector Exchange Intune la premisa
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808144"
---
# <a name="intune-exchange-on-premise-connector"></a>Conector Exchange Intune la premisa

Pentru detalii despre Configurarea conectorului între Intune și Exchange găzduit local, vă rugăm să consultați următoarea documentație:

[Configurarea conectorului Exchange local Intune în Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ**

Î: văd o eroare, cum ar fi "versiunea conectorului Exchange nu este acceptată" atunci când încercați să configurați conectorul Exchange. Care ar putea fi cauza?

A: contul pe care îl utilizați este licențiat corespunzător-trebuie să aibă o licență Intune activă

Î: este posibil să aveți mai mulți conectori Exchange?

A: puteți să configurați un singur conector Exchange per Intune entitate găzduită per organizație Exchange. Conectorul poate fi instalat doar pe un server într-o organizație Exchange pentru mai multe servere.

De asemenea, nu este posibil să aveți conectori configurați pentru Exchange local și Exchange Online configurate în aceeași entitate găzduită.

Î: poate conectorul să utilizeze o matrice CAS ca conexiune la Exchange?

A: specificarea unei matrice CAS nu este o configurație acceptată în Configurarea conectorului. Trebuie specificat doar un singur server și ar trebui să fie hardcoded în fișierul de configurare a conectorului care poate fi găsit în

program data\microsoft\microsoft Intune pe conector Exchange premisă \ OnpremiseExchangeConnectorServiceConfiguration.xml

Găsiți următoarea intrare ```<ExchangeWebServiceURL />``` și înlocuiți URL-ul cu serverul Exchange.

**Exemplu**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consultați următoarea documentație pentru depanare suplimentară: [Depanarea conectorului Exchange local Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Activarea înregistrării în jurnal detaliată pentru conectorul Exchange**

1. Deschideți fișierul de configurare de urmărire a conectorului Exchange pentru editare.  
Fișierul este localizat la adresa:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exemplu**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Găsiți TraceSourceLine cu următoarea cheie: OnPremisesExchangeConnectorService  
  
3. Modificarea valorii nodului SourceLevel din ActivityTracing de informații (setarea implicită) la ActivityTracing detaliată  

**Exemplu**
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
4. Reporniți serviciul Exchange Microsoft Intune  
5. Sincronizare completă în portalul Intune până când se termină, apoi modificați XML-ul înapoi la "informații ActivityTracing" și reporniți serviciul Exchange Microsoft Intune.  
6. Locația jurnalelor este: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`