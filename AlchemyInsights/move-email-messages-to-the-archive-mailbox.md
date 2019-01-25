---
title: Muta mesajele de e-mail către cutia poştală de arhivă
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485291"
---
<span data-ttu-id="451c2-p101">Probleme de arhivare elementele în cutia poştală de arhivă. Asiguraţi-vă că aţi parcurs paşii de mai jos:</span><span class="sxs-lookup"><span data-stu-id="451c2-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="451c2-p102">Confirmaţi că o **Arhiva cutie poştală** a fost activată. Dacă nu, utilizaţi paşii din [acest articol](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) pentru a permite cutiei poştale de arhivă.</span><span class="sxs-lookup"><span data-stu-id="451c2-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="451c2-106">În centrul de administrare Exchange, selectaţi **Etichetele de conservare** , sub **Managementul de conformitate**, creaţi o **etichetă de conservare** cu acţiunea **trece la Arhiva** conţinând dorit de **Vechime de conservare**.</span><span class="sxs-lookup"><span data-stu-id="451c2-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="451c2-107">În centrul de administrare Exchange, selectaţi **Strategiile de conservare**, crea o **Strategie de conservare** şi se adaugă vă **trece la Arhiva** etichetă de conservare a acestei politici.</span><span class="sxs-lookup"><span data-stu-id="451c2-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="451c2-p103">[Atribui conservare](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) la cutia poştală a utilizatorului specifice. Aceeaşi politică va aplica atât **primare** şi cutia poştală de **arhivă** .</span><span class="sxs-lookup"><span data-stu-id="451c2-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="451c2-p104">Cutia poştală a utilizatorului acum ar trebui să aibă o politică de Arhiva să mutaţi elementele în cutia poştală de arhivă. Este necesar să se vigoare reuşit Folder asistent (MAE) pentru a rula şi de a aplica noile setări pentru cutia poştală a utilizatorului. Executaţi următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poştală:</span><span class="sxs-lookup"><span data-stu-id="451c2-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="451c2-113">Doresc mai multe informaţii privind înfiinţarea unei politici de arhiva, a se vedea [Configurarea unei politici Arhiva şi ştergere pentru cutii poştale](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="451c2-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

