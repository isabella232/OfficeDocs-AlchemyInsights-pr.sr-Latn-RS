---
title: Identifikovanje događaja brisanja poruka u evidenciji nadzora
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696527"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="e9ca1-102">Evidencija nadzora za izbrisane e-poruke</span><span class="sxs-lookup"><span data-stu-id="e9ca1-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="e9ca1-103">Počevši od januara 2019, Microsoft automatski pokreće Office proveru poštanskog sandučeta.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="e9ca1-104">U suprotnom, da biste pregledali brisanje događaja poruke za određenog korisnika, morate ručno da omogućite radnje brisanja za nadgledanje.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="e9ca1-105">Ako je evidentiranje nadzora poštanskog sandučeta već omogućeno za vašu organizaciju ili za određenog korisnika, slijedite dolenavedene korake.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="e9ca1-106">Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e9ca1-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="e9ca1-107">Izaberite stavku **Pretraga i istraga** i izaberite stavku **Pretraga evidencije nadzora**.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="e9ca1-108">Izaberite opseg datuma u poljima **početni** i **Krajnji datum** .</span><span class="sxs-lookup"><span data-stu-id="e9ca1-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e9ca1-109">Navedite korisničko ime za korisnika koga želite da istražite (korisnik koji je izbrisao stavke).</span><span class="sxs-lookup"><span data-stu-id="e9ca1-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="e9ca1-110">U polju **aktivnosti** izaberite stavku **izbrisane poruke iz fascikle "Izbrisane stavke"** i **premestili poruke u fasciklu "Izbrisane stavke**".</span><span class="sxs-lookup"><span data-stu-id="e9ca1-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="e9ca1-111">Kliknite na dugme **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-111">Click **Search**.</span></span>

<span data-ttu-id="e9ca1-112">U rezultatima izaberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-112">In the results, select an audit record.</span></span> <span data-ttu-id="e9ca1-113">U okviru detalji, kliknite na dugme **više informacija**.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e9ca1-114">Dodatne informacije o izbrisanom artiklu (na primer, redu za temu i lokacija stavke kada je izbrisana) prikazuje se u polju " **Afekcteditem** ".</span><span class="sxs-lookup"><span data-stu-id="e9ca1-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="e9ca1-115">**ClientInfoString** će se prikazati ako je brisanje došlo u programu Outlook, Outlook na vebu (ranije ime Outlook Web App) ili bilo kom drugom uređaju.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="e9ca1-116">Više informacija potražite u članku [Utvrđivanje ko je podesio Prosleđivanje e-pošte za poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="e9ca1-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="e9ca1-117">**Napomena**: ne možete da preuzmete izbrisane stavke pomoću funkcije evidencije nadzora.</span><span class="sxs-lookup"><span data-stu-id="e9ca1-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="e9ca1-118">Da biste preuzeli izbrisane poruke u programu Outlook na vebu, pogledajte članak [oporavak izbrisanih stavki u programu Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="e9ca1-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
