---
title: ADFS certifikat za u federation expiring
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952983"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS certifikat za u federation expiring

Da biste rešili ovaj problem, pratite ove korake:
  
1. Instalirajte Microsoft Azure Active Directory modul za Windows PowerShell na računaru (ako modul nije već instaliran). Da biste to uradio, idite [na upravljanje uslugom Azure AD pomoću Windows PowerShell.](https://aka.ms/aadposh)

2. Pratite korake u odeljku "1. slučaj: Istekao je certifikat za potpisivanje AD FS tokena" u odeljku "Došlo je do problema sa pristupom sajtu" iz AD FS kada se federan korisnik prijavi u [Microsoft 365, Azure ili Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Pratite korake u članku Ažuriranje ili popravljanje postavki federanog domena u uslugama [Microsoft, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Da biste saznali više o obnavljanju certifikata za federation, pogledajte obnavljanje certifikata za federation [za Microsoft 365 i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
