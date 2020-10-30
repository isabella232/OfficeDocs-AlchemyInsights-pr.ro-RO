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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="d9895-102">Conector Exchange Intune la premisa</span><span class="sxs-lookup"><span data-stu-id="d9895-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="d9895-103">Pentru detalii despre Configurarea conectorului între Intune și Exchange găzduit local, vă rugăm să consultați următoarea documentație:</span><span class="sxs-lookup"><span data-stu-id="d9895-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="d9895-104">Configurarea conectorului Exchange local Intune în Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="d9895-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="d9895-105">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="d9895-105">**FAQ:**</span></span>

<span data-ttu-id="d9895-106">Î: văd o eroare, cum ar fi "versiunea conectorului Exchange nu este acceptată" atunci când încercați să configurați conectorul Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9895-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="d9895-107">Care ar putea fi cauza?</span><span class="sxs-lookup"><span data-stu-id="d9895-107">What could be the cause?</span></span>

<span data-ttu-id="d9895-108">A: contul pe care îl utilizați este licențiat corespunzător-trebuie să aibă o licență Intune activă</span><span class="sxs-lookup"><span data-stu-id="d9895-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="d9895-109">Î: este posibil să aveți mai mulți conectori Exchange?</span><span class="sxs-lookup"><span data-stu-id="d9895-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="d9895-110">A: puteți să configurați un singur conector Exchange per Intune entitate găzduită per organizație Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9895-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="d9895-111">Conectorul poate fi instalat doar pe un server într-o organizație Exchange pentru mai multe servere.</span><span class="sxs-lookup"><span data-stu-id="d9895-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="d9895-112">De asemenea, nu este posibil să aveți conectori configurați pentru Exchange local și Exchange Online configurate în aceeași entitate găzduită.</span><span class="sxs-lookup"><span data-stu-id="d9895-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="d9895-113">Î: poate conectorul să utilizeze o matrice CAS ca conexiune la Exchange?</span><span class="sxs-lookup"><span data-stu-id="d9895-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="d9895-114">A: specificarea unei matrice CAS nu este o configurație acceptată în Configurarea conectorului.</span><span class="sxs-lookup"><span data-stu-id="d9895-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="d9895-115">Trebuie specificat doar un singur server și ar trebui să fie hardcoded în fișierul de configurare a conectorului care poate fi găsit în</span><span class="sxs-lookup"><span data-stu-id="d9895-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="d9895-116">program data\microsoft\microsoft Intune pe conector Exchange premisă \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="d9895-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="d9895-117">Găsiți următoarea intrare ```<ExchangeWebServiceURL />``` și înlocuiți URL-ul cu serverul Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9895-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="d9895-118">**Exemplu**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="d9895-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="d9895-119">Consultați următoarea documentație pentru depanare suplimentară: [Depanarea conectorului Exchange local Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="d9895-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="d9895-120">**Activarea înregistrării în jurnal detaliată pentru conectorul Exchange**</span><span class="sxs-lookup"><span data-stu-id="d9895-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="d9895-121">Deschideți fișierul de configurare de urmărire a conectorului Exchange pentru editare.</span><span class="sxs-lookup"><span data-stu-id="d9895-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="d9895-122">Fișierul este localizat la adresa:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="d9895-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="d9895-123">**Exemplu**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="d9895-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="d9895-124">Găsiți TraceSourceLine cu următoarea cheie: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="d9895-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="d9895-125">Modificarea valorii nodului SourceLevel din ActivityTracing de informații (setarea implicită) la ActivityTracing detaliată</span><span class="sxs-lookup"><span data-stu-id="d9895-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="d9895-126">**Exemplu**</span><span class="sxs-lookup"><span data-stu-id="d9895-126">**Example:**</span></span>
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
4. <span data-ttu-id="d9895-127">Reporniți serviciul Exchange Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9895-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="d9895-128">Sincronizare completă în portalul Intune până când se termină, apoi modificați XML-ul înapoi la "informații ActivityTracing" și reporniți serviciul Exchange Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d9895-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="d9895-129">Locația jurnalelor este: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="d9895-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>