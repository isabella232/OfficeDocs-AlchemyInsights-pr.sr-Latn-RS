---
title: Rešavanje problema sa hibridnim pridruživanjem u usluzi Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401921"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Rešavanje problema sa hibridnim pridruživanjem u usluzi Azure AD

Preporučuje se da se pobrinete da uređaj može da pristupi krajnjim tačkama registracije uređaja u okviru sistemskog naloga koristeći [skriptu za test povezivanja registracije uređaja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Ako prvi put podešavate registracije uređaja, obavezno pregledajte [Uvod u upravljanje uređajima u usluzi Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) da biste saznali kako da stavite uređaje pod kontrolu usluge Azure AD.
1. Ako registrujete uređaje direktno u Azure AD i upišete ih u Intune, najpre se uverite da ste [konfigurisali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da je [licenciranje](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) spremno.
1. Uverite se da ste ovlašćeni za izvršavanje operacija u usluzi Azure AD i lokalnom AD. Postavkama za registracije uređaja može da upravlja samo globalni administrator u usluzi Azure AD. Pored toga, ako podešavate automatske registracije u lokalnom aktivnom direktorijumu, moraćete da budete administrator za aktivni direktorijum i AD FS (ako je primenljivo).

Za više detalja o rešavanju potencijalnih problema sa hibridnim pridruživanjem, pogledajte [Rešavanje problema sa hibridnim pridruživanjem](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) za podešavanje hibridnih uređaja pridruženih putem usluge Azure AD i upravljanje uređajima pomoću Azure AD portala, pogledajte [Podešavanje hibridnih uređaja pridruženih putem usluge Azure AD (lokalnih uređaja pridruženih u domenu)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) i [Upravljanje uređajima putem Azure portala](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Da biste rešili uobičajene probleme sa hibridnim pridruživanjem putem usluge Azure Active Directory (AD), pogledajte [Najčešća pitanja u vezi sa hibridnim pridruživanjem putem usluge Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
