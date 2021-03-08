---
title: Konfigurisanje šifrovanja poruka za hibridno okruženje
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526600"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="9ba33-102">Konfigurisanje šifrovanja poruka za hibridno okruženje</span><span class="sxs-lookup"><span data-stu-id="9ba33-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="9ba33-103">Za hibridna okruženja, korisnici lokalnog sistema mogu da šalju šifrovanu e-poštu pomoću šifrovanja Office poruke (OME) samo ako se e-pošta usmerava putem usluge Exchange online.</span><span class="sxs-lookup"><span data-stu-id="9ba33-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="9ba33-104">Da biste Šifruj e-poruke pomoću Oma, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="9ba33-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="9ba33-105">Koristite [čarobnjak za hibridnu konfiguraciju](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) da biste podesili hibridno okruženje.</span><span class="sxs-lookup"><span data-stu-id="9ba33-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="9ba33-106">Nisu neophodni posebni koraci za podešavanje šifrovanja.</span><span class="sxs-lookup"><span data-stu-id="9ba33-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="9ba33-107">[Podesite pravila protoka pošte za šifrovanje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) kao što to obično radite.</span><span class="sxs-lookup"><span data-stu-id="9ba33-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


