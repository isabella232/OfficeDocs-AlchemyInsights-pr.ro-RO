---
title: Problemă la asocierea la VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885664"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="534b1-102">Problemă la asocierea la VMs</span><span class="sxs-lookup"><span data-stu-id="534b1-102">Issue joining VMs</span></span>

<span data-ttu-id="534b1-103">Pentru a rezolva problemele care apar când încercați să vă asociați la VMs, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="534b1-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="534b1-104">Încercați să vă conectați utilizând formatul **UPN** (de exemplu, "JoeUser@contoso.com") în loc de formatul **sAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="534b1-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="534b1-105">Asigurați-vă că ați activat sincronizarea parolei în conformitate cu pașii schițați *în Ghidul introductiv* .</span><span class="sxs-lookup"><span data-stu-id="534b1-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="534b1-106">Asigurați-vă că contul de utilizator afectat nu este un cont extern în entitatea găzduită Azure AD.</span><span class="sxs-lookup"><span data-stu-id="534b1-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="534b1-107">Utilizatorii externi nu se pot conecta la domeniul gestionat deoarece serviciile de domeniu Azure AD nu au acreditări pentru astfel de conturi de utilizator.</span><span class="sxs-lookup"><span data-stu-id="534b1-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="534b1-108">Dacă contul de utilizator afectat este un cont de utilizator în cloud, asigurați-vă că utilizatorii și-au schimbat parola după ce ați activat serviciile de domeniu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="534b1-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="534b1-109">Acest pas determină hash-ul de acreditări necesar pentru ca serviciile de domeniu Azure AD să fie generate.</span><span class="sxs-lookup"><span data-stu-id="534b1-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="534b1-110">Dacă conturile de utilizator afectate sunt sincronizate dintr-un director local, Verificați dacă a fost configurată versiunea recomandată de Azure AD Connect pentru a efectua o sincronizare completă.</span><span class="sxs-lookup"><span data-stu-id="534b1-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="534b1-111">Dacă problemele persistă după ce confirmați pasul 4, efectuați următoarele comenzi de la mașina de sincronizare:</span><span class="sxs-lookup"><span data-stu-id="534b1-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="534b1-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="534b1-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>