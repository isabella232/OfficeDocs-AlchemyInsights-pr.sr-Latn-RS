---
title: Intune Exchange -besmisleni konektor
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
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013978"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange -besmisleni konektor

Detalje podešavanja konektora između usluge Intune i usluge Exchange koja se hostuje besmisleno potražite u sledećoj dokumentaciji:

[Podešavanje Exchange Intune konektora u Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Faq:**

P: Vidim grešku kao što je "Verzija Exchange Connector nije podržana" prilikom pokušaja postavljanja konektora Exchange podataka. Koji uzrok može da bude?

O: Nalog koji koristite je licenciran na odgovarajući način – mora da ima aktivnu Intune licencu

P: Da li je moguće imati više konektora Exchange više?

O: Možete da podesite samo jedan konektor Exchange po Intune zakuponu po Exchange organizaciji. Konektor može da se instalira samo na jednom serveru u organizaciji sa više servera.

Takođe, nije moguće podesiti konektore konfigurisane za Exchange i za Exchange Online konfigurisan u istom zakupca.

P: Da li konektor može da koristi CAS niz kao vezu sa Exchange?

O: Navođenje CAS niza nije podržana konfiguracija u instalaciji konektora. Samo jedan server treba da bude naveden i trebalo bi ga čvrsto koditi u konfiguracionoj datoteci konektora koju je moguće pronaći u

podaci programa\microsoft\microsoft Intune (Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Pronađite sledeću ```<ExchangeWebServiceURL />``` stavku i zamenite URL sa Exchange serverom.

**Primer:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Pogledajte sledeću dokumentaciju za dodatno rešavanje problema: Rešavanje problema sa Exchange [Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Omogućavanje evidentiranje pomoću "pošiljalaca" Exchange spajanja**

1. Otvorite konfiguracionu datoteku Exchange Connector tracing radi uređivanja.  
Datoteka se nalazi na lokaciji: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Primer:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Pronađite TraceSourceLine sledećim ključem: OnPremisesExchangeConnectorService  
  
3. Promena vrednosti SourceLevel node sa Information ActivityTracing (podrazumevano) na "Rebose ActivityTracing"  

**Primer:**
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
4. Ponovo pokrenite Microsoft Intune Exchange Usluge  
5. Potpuna sinhronizacija na Intune portalu dok se ne završi, a zatim vratite XML u "Information ActivityTracing" i ponovo pokrenite Microsoft Intune Exchange Service.  
6. Lokacija evidencija je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`