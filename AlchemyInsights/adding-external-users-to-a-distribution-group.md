---
title: Adăugarea utilizatorilor externi la un grup de distribuire
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663525"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="826c8-102">Adăugarea utilizatorilor externi la un grup de distribuire</span><span class="sxs-lookup"><span data-stu-id="826c8-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="826c8-103">Adăugarea unei persoane de contact externe la un grup de distribuire (DG) este un proces în doi pași:</span><span class="sxs-lookup"><span data-stu-id="826c8-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="826c8-104">Creați o persoană de contact de E-mail pentru utilizatorul extern:</span><span class="sxs-lookup"><span data-stu-id="826c8-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="826c8-105">În centrul de administrare, accesați **Users**  >  pagina[persoane de contact](https://admin.microsoft.com/adminportal/home#/Contact) pentru utilizatori.</span><span class="sxs-lookup"><span data-stu-id="826c8-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="826c8-106">Selectați **Adăugați o persoană de contact**.</span><span class="sxs-lookup"><span data-stu-id="826c8-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="826c8-107">Tastați informațiile pentru persoana de contact și selectați **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="826c8-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="826c8-108">Adăugați persoana de contact de E-mail la DG:</span><span class="sxs-lookup"><span data-stu-id="826c8-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="826c8-109">În centrul de administrare, accesați pagina grupuri **grupuri**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="826c8-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="826c8-110">Găsiți DG-ul la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide caseta de dialog Editare.</span><span class="sxs-lookup"><span data-stu-id="826c8-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="826c8-111">Pe fila **Membri** , selectați **Vizualizați toți și gestionați membri**.</span><span class="sxs-lookup"><span data-stu-id="826c8-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="826c8-112">Selectați **Adăugare membri**.</span><span class="sxs-lookup"><span data-stu-id="826c8-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="826c8-113">Selectați persoana de contact de E-mail pe care ați creat-o la pasul anterior, apoi selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="826c8-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="826c8-114">Dacă după ce urmați acești pași, utilizatorii externi nu pot trimite mesaje de e-mail către DG sau nu primesc mesaje de e-mail de la acesta, ar putea fi faptul că DG este marcată pentru a permite doar mesajele de e-mail de la utilizatorii interni.</span><span class="sxs-lookup"><span data-stu-id="826c8-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="826c8-115">Puteți să verificați această configurație și să o remediați urmând instrucțiunile de [aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="826c8-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="826c8-116">**Notă:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "Microsoft 365 Group" în loc de "grup de distribuire".</span><span class="sxs-lookup"><span data-stu-id="826c8-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="826c8-117">Dacă acesta este cazul, puteți adăuga utilizatorul extern direct la grup din Outlook.</span><span class="sxs-lookup"><span data-stu-id="826c8-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="826c8-118">Informații detaliate despre Microsoft 365 Groups invitati, precum și instrucțiuni pentru adăugarea oaspeților externi pot fi găsiți în [acest articol](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="826c8-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  