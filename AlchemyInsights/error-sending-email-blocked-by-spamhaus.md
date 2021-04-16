---
title: Eroare de trimitere a e-mailului blocat de SpamHaus
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
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813736"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f20cc-102">Eroare de trimitere e-mail: Gazda client blocată utilizând Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f20cc-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f20cc-103">Adresa IP de la care a fost trimis mesajul se află pe o listă de blocări deținută [de Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f20cc-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f20cc-104">Între motivele pentru blocarea de către Spamhaus sunt incluse conturi compromise, mașini compromise care partajează o adresă IP publică și politici ale unui furnizor de servicii internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="f20cc-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f20cc-105">Remedierile posibile sunt:</span><span class="sxs-lookup"><span data-stu-id="f20cc-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f20cc-106">Pentru mesajele de intrare blocate, în care puteți controla serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocarea din site-ul web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f20cc-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f20cc-107">Pentru mesajele de intrare către care adresa IP sursă aparține altcuiva, proprietarul adresei trebuie să elimine blocarea din site-ul web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f20cc-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f20cc-108">Dacă adresa IP este pe Lista de blocare de politică (PBL - Policy Block List), proprietarul poate să atribuie o adresă IP statică diferită sau să elimine adresa din PBL.</span><span class="sxs-lookup"><span data-stu-id="f20cc-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f20cc-109">Pentru mesajele de ieșire blocate din domeniul dvs. conectat la Microsoft, puteți primi această eroare dacă mesajele sunt distribuite printr-un serviciu terț.</span><span class="sxs-lookup"><span data-stu-id="f20cc-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f20cc-110">Puteți utiliza un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.</span><span class="sxs-lookup"><span data-stu-id="f20cc-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
