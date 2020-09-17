---
title: Eroare la trimiterea e-mailului blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783815"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f339d-102">Eroare la trimiterea mesajelor de e-mail: gazdă client blocată utilizând Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f339d-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f339d-103">Adresa IP care a trimis mesajul se află într-o listă de blocări deținută de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f339d-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f339d-104">Motivele pentru care sunt blocate de Spamhaus includ conturi compromise, mașini compromise care partajează o adresă IP publică și politici de furnizor de servicii Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="f339d-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f339d-105">Remedieri posibile sunt:</span><span class="sxs-lookup"><span data-stu-id="f339d-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f339d-106">Pentru mesajele de intrare blocate în care controlați serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocul din site-ul web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f339d-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f339d-107">Pentru mesajele de intrare blocate în care adresa IP sursă aparține altei persoane, proprietarul adresei trebuie să elimine blocul din site-ul web Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f339d-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f339d-108">Dacă adresa IP este pe lista de politici Block (PBL), proprietarul poate atribui o altă adresă IP statică sau elimina adresa din PBL.</span><span class="sxs-lookup"><span data-stu-id="f339d-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f339d-109">Pentru mesajele de ieșire blocate din domeniul conectat la Microsoft, puteți primi această eroare dacă mesajele sunt direcționate prin intermediul unui serviciu 3rd party.</span><span class="sxs-lookup"><span data-stu-id="f339d-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f339d-110">Puteți utiliza un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.</span><span class="sxs-lookup"><span data-stu-id="f339d-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
