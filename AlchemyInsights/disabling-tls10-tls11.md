---
title: Zabrana prosleđivanja TLS1.0 i TLS 1.1 za prosleđivanje SMTP AUTH klijenta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455123"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Zabrana prosleđivanja TLS1.0 i TLS 1.1 za prosleđivanje SMTP AUTH klijenta

Nedavno smo počeli da zabranjemo prosleđivanje TLS1.0 i TLS 1.1 za prosleđivanje SMTP AUTH klijenta. 

Ako ste konfigurisali uređaj, aplikaciju ili server koji šalje e-poštu u uslugu Microsoft 365 koristeći metod prosleđivanja SMTP AUTH klijenta, uverite se da uređaj, aplikacija ili server podržavaju TLS 1.2 za SMTP. 