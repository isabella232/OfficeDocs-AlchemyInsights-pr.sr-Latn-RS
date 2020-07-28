---
title: Promena kanala za ažuriranje Office aplikacija
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440019"
---
# <a name="change-update-channels-for-office-apps"></a>Promena kanala za ažuriranje Office aplikacija

Za nove Office instalacije koristite postavke za preuzimanje Office softvera da biste izabrali željeni kanal za ažuriranje, a zatim instalirali (ili ponovo instalirajte) Office aplikacije. Više informacija potražite u članku [Upravljanje postavkama za preuzimanje softvera u sistemu Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Belešku** Kanal za ažuriranje koji je izabran pomoću postavki za preuzimanje Office softvera primenjuje se na sve korisnike koji vrše nove instalacije pomoću O365 portala. Više informacija potražite u članku [Preuzimanje i instaliranje ili ponovna instalacija sistema Microsoft 365 ili Office 2019 na računaru ili Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)računarima.   

Za postojeće Office instalacije koristite alatku za primenu sistema Office (ODT) za prebacivanje na drugi kanal za ažuriranje:  

1. Preuzmite najnoviju verziju alatke za primenu sistema Office (setup.exe) sa [lokacije Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifikujte ime kanala na koji želite da pređete. Više informacija potražite u članku [opcije konfiguracije za alatku za primenu sistema Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Kreirajte XML datoteku za konfiguraciju koja navodi odgovarajuće ime kanala, na primer update.xml.  
    A. <Configuration>  
    B. <dopune **kanal = "mesečno"** />  
    C. </Configuration>
4. Na osnovu pune komandne linije prebacite se na lokaciju fascikle na kojoj setup.exe nalazi i pokrenite sledeću komandu:  
    A. setup.exe/Konfiguriši update.xml
5. Pokrenite Office aplikaciju (kao što je Excel), a zatim izaberite **File**  >  **nalog**datoteka. U odeljku informacije o proizvodu izaberite stavku **Ažuriraj opcije**  >  **Ažuriraj odmah**.

Za više informacija pogledajte odeljak [Kako da promenite ažuriranje kanala za postojeće Office aplikacije](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Za prebacivanje na kanale za izabranu grupu korisnika ili pomoću upravljača konfiguracije (SCCM) Konfigurišite postavku za ažuriranje kanala pomoću GPO-a. Više informacija potražite u članku [Prikaz kanala za ažuriranje Microsoft 365 aplikacija](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Više informacija potražite u članku [Kako da upravljate kanalima Office 365 ProPlus za IT stručnjake](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) i [da upravljate ispravkama za Microsoft 365 aplikacije pomoću upravljača za konfiguraciju krajnje tačke na lokaciji Microsoft](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).