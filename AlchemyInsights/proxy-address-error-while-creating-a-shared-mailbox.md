---
title: Eroare de adresă proxy în timp ce creați o cutie poștală partajată
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568302"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="59ea5-102">Eroare de adresă proxy în timp ce creați o cutie poștală sau alt obiect activat pentru e-mail</span><span class="sxs-lookup"><span data-stu-id="59ea5-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="59ea5-103">Dacă ați încercat să creați un obiect activat pentru e-mail (cutie poștală, cutie poștală partajată etc.) și ați primit eroarea "adresa proxy" SMTP:alias@domain.com "este deja utilizată...", adresa de e-mail pe care ați ales-o este deja luată de un alt obiect activat pentru e-mail din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="59ea5-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="59ea5-104">Trebuie să găsiți utilizatorul, grupul, cutia poștală partajată sau folderul public care are această adresă de e-mail și să o șteargă sau să își modifice adresa de e-mail.</span><span class="sxs-lookup"><span data-stu-id="59ea5-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="59ea5-105">Apoi puteți crea un nou obiect activat pentru e-mail cu adresa de e-mail gratuită.</span><span class="sxs-lookup"><span data-stu-id="59ea5-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="59ea5-106">Utilizați căutare pe pagina de pornire pentru a o găsi.</span><span class="sxs-lookup"><span data-stu-id="59ea5-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="59ea5-107">De asemenea, puteți utiliza următoarea comandă PowerShell Exchange Online pentru a o căuta:</span><span class="sxs-lookup"><span data-stu-id="59ea5-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="59ea5-108">Dacă nu doriți să ștergeți adresa de e-mail existentă, alegeți o nouă adresă de e-mail pentru obiectul nou pe care îl creați.</span><span class="sxs-lookup"><span data-stu-id="59ea5-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  