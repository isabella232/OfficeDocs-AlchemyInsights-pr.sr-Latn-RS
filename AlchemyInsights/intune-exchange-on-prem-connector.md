---
title: Intune Exchange konektor
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
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808143"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="1c12a-102">Intune Exchange konektor</span><span class="sxs-lookup"><span data-stu-id="1c12a-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="1c12a-103">Detalje o podešavanju konektora između Intune i razmene koji se hostujete u lokalnom članku potražite u sledećoj dokumentaciji:</span><span class="sxs-lookup"><span data-stu-id="1c12a-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="1c12a-104">Podešavanje lokalnog Exchange konektora Intune u programu Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="1c12a-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="1c12a-105">**NAJČEŠĆA pitanja**</span><span class="sxs-lookup"><span data-stu-id="1c12a-105">**FAQ:**</span></span>

<span data-ttu-id="1c12a-106">P: vidim grešku kao što je "verzija Exchange konektora nije podržana" prilikom pokušaja podešavanja Exchange konektora.</span><span class="sxs-lookup"><span data-stu-id="1c12a-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="1c12a-107">Šta može da bude uzrok?</span><span class="sxs-lookup"><span data-stu-id="1c12a-107">What could be the cause?</span></span>

<span data-ttu-id="1c12a-108">A: nalog koji koristite je licenciran na odgovarajući način – mora da ima aktivnu licencu za Intune</span><span class="sxs-lookup"><span data-stu-id="1c12a-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="1c12a-109">Q: da li je moguće imati više Exchange konektora?</span><span class="sxs-lookup"><span data-stu-id="1c12a-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="1c12a-110">A: možete da podesite samo jedan Exchange konektor po Intune stanari po Exchange organizaciji.</span><span class="sxs-lookup"><span data-stu-id="1c12a-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="1c12a-111">Konektor može da se instalira samo na jednom serveru u Exchange organizaciji multi server.</span><span class="sxs-lookup"><span data-stu-id="1c12a-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="1c12a-112">Takođe, ne možete da imate konektore podešene za razmenu na mreži i Exchange online konfigurisani u istom zakupcu.</span><span class="sxs-lookup"><span data-stu-id="1c12a-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="1c12a-113">Q: da li konektor može da koristi niz Kas kao vezu sa Exchange serverom?</span><span class="sxs-lookup"><span data-stu-id="1c12a-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="1c12a-114">A: Navođenje niza Kas Kas nije podržana konfiguracija u podešavanju konektora.</span><span class="sxs-lookup"><span data-stu-id="1c12a-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="1c12a-115">Samo jedan server treba da bude naveden i treba da bude u okviru datoteke konfiguracije konektora koji se može pronaći u</span><span class="sxs-lookup"><span data-stu-id="1c12a-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="1c12a-116">programdata\microsoft\microsoft Intune na lokalno Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="1c12a-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="1c12a-117">Pronađite sledeću stavku ```<ExchangeWebServiceURL />``` i zamenite URL adresu Exchange serverom.</span><span class="sxs-lookup"><span data-stu-id="1c12a-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="1c12a-118">**Primer**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="1c12a-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="1c12a-119">Pogledajte sledeću dokumentaciju za dodatnu rešavanje problema: [Rešavanje problema sa Intune lokalno Exchange konektorom](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="1c12a-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="1c12a-120">**Omogućavanje ispravnog vođenja evidencije za Exchange konektor**</span><span class="sxs-lookup"><span data-stu-id="1c12a-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="1c12a-121">Otvorite datoteku konfiguracije praćenja Exchange konektora za uređivanje.</span><span class="sxs-lookup"><span data-stu-id="1c12a-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="1c12a-122">Datoteka se nalazi na lokaciji:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="1c12a-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="1c12a-123">**Primer**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="1c12a-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="1c12a-124">Pronađite Tracesourselin sa sledećim ključem: Onpremisesexchangeonline Service</span><span class="sxs-lookup"><span data-stu-id="1c12a-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="1c12a-125">Promena vrednosti čvora SourceLevel iz praćenja Aktivacijefunkcija (podrazumevano) za verbalno Aktivacijepraćenje</span><span class="sxs-lookup"><span data-stu-id="1c12a-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="1c12a-126">**Primer**</span><span class="sxs-lookup"><span data-stu-id="1c12a-126">**Example:**</span></span>
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
4. <span data-ttu-id="1c12a-127">Ponovno pokretanje usluge Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="1c12a-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="1c12a-128">Potpuna sinhronizacija u Intune Portovu dok se ne završi, a zatim ponovo promenite XML u "aktivaciju podataka" i ponovo pokrenite Exchange Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c12a-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="1c12a-129">Lokacija evidencija je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="1c12a-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>