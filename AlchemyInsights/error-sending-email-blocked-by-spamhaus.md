---
title: Eroare la trimiterea e-mailului blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714270"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f557c-102">Eroare la trimiterea e-mailului: Client gazdă blocat folosind Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f557c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f557c-103">Adresa IP care a trimis mesajul este pe o listă de bloc deținute de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f557c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f557c-104">Motivele pentru care a fost blocat de Spamhaus includ conturi compromise, mașini compromise care partajează o adresă IP publică și politici de furnizor de servicii internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="f557c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f557c-105">Remedierile posibile sunt:</span><span class="sxs-lookup"><span data-stu-id="f557c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f557c-106">Pentru mesajele de intrare blocate în cazul în care controlați serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocul de pe site-ul Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f557c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f557c-107">Pentru mesajele de intrare blocate în cazul în care adresa IP sursă aparține altcuiva, proprietarul adresei trebuie să elimine blocul de pe site-ul Web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f557c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f557c-108">Dacă adresa IP se află în Lista de blocărărilor de politici (PBL), proprietarul poate atribui o altă adresă IP statică sau poate elimina adresa din PBL.</span><span class="sxs-lookup"><span data-stu-id="f557c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f557c-109">Pentru mesajele de ieșire blocate din domeniul conectat la Microsoft, puteți primi această eroare dacă mesajele sunt distribuite printr-un serviciu terț.</span><span class="sxs-lookup"><span data-stu-id="f557c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f557c-110">Utilizați un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.</span><span class="sxs-lookup"><span data-stu-id="f557c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
