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
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange konektor

Detalje o podešavanju konektora između Intune i razmene koji se hostujete u lokalnom članku potražite u sledećoj dokumentaciji:

[Podešavanje lokalnog Exchange konektora Intune u programu Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**NAJČEŠĆA pitanja**

P: vidim grešku kao što je "verzija Exchange konektora nije podržana" prilikom pokušaja podešavanja Exchange konektora. Šta može da bude uzrok?

A: nalog koji koristite je licenciran na odgovarajući način – mora da ima aktivnu licencu za Intune

Q: da li je moguće imati više Exchange konektora?

A: možete da podesite samo jedan Exchange konektor po Intune stanari po Exchange organizaciji. Konektor može da se instalira samo na jednom serveru u Exchange organizaciji multi server.

Takođe, ne možete da imate konektore podešene za razmenu na mreži i Exchange online konfigurisani u istom zakupcu.

Q: da li konektor može da koristi niz Kas kao vezu sa Exchange serverom?

A: Navođenje niza Kas Kas nije podržana konfiguracija u podešavanju konektora. Samo jedan server treba da bude naveden i treba da bude u okviru datoteke konfiguracije konektora koji se može pronaći u

programdata\microsoft\microsoft Intune na lokalno Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Pronađite sledeću stavku ```<ExchangeWebServiceURL />``` i zamenite URL adresu Exchange serverom.

**Primer**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Pogledajte sledeću dokumentaciju za dodatnu rešavanje problema: [Rešavanje problema sa Intune lokalno Exchange konektorom](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Omogućavanje ispravnog vođenja evidencije za Exchange konektor**

1. Otvorite datoteku konfiguracije praćenja Exchange konektora za uređivanje.  
Datoteka se nalazi na lokaciji:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Primer**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Pronađite Tracesourselin sa sledećim ključem: Onpremisesexchangeonline Service  
  
3. Promena vrednosti čvora SourceLevel iz praćenja Aktivacijefunkcija (podrazumevano) za verbalno Aktivacijepraćenje  

**Primer**
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
4. Ponovno pokretanje usluge Microsoft Intune Exchange  
5. Potpuna sinhronizacija u Intune Portovu dok se ne završi, a zatim ponovo promenite XML u "aktivaciju podataka" i ponovo pokrenite Exchange Microsoft Intune Exchange.  
6. Lokacija evidencija je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`