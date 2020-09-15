---
title: 1554 Winsock greška 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698876"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="4b691-102">Winsock greška 10061</span><span class="sxs-lookup"><span data-stu-id="4b691-102">Winsock error 10061</span></span>

<span data-ttu-id="4b691-103">Ovaj kôd greške znači da Microsoft nije mogao da uspostavi TCP priključak (vezu) sa ciljem ciljnog domaćina.</span><span class="sxs-lookup"><span data-stu-id="4b691-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="4b691-104">Najverovatniji uzrok ove greške je problem sa konfiguracijom zaštitnog zida.</span><span class="sxs-lookup"><span data-stu-id="4b691-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="4b691-105">Da biste rešili problem, potvrdite izbor u ovim postavkama:</span><span class="sxs-lookup"><span data-stu-id="4b691-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="4b691-106">Verifikacija konfiguracije zaštitnog zida pomoću informacija u [Microsoft 365 URL adresama i opsezima IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="4b691-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="4b691-107">Ako je greška karakteristična za Exchange online Protection (EOP), trebalo je da budete prethodno obavešteni na [IP adrese Exchange online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="4b691-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="4b691-108">Potvrdite da dobavljač Internet usluga (ISP) ne blokira port.</span><span class="sxs-lookup"><span data-stu-id="4b691-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="4b691-109">Potvrdite pametne postavke domaćina i odredišne servere u konektorima.</span><span class="sxs-lookup"><span data-stu-id="4b691-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="4b691-110">Imajte na umu da Microsoft 365 ne blokira *dolazne* veze na ovaj način.</span><span class="sxs-lookup"><span data-stu-id="4b691-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
