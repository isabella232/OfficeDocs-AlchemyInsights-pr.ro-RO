---
title: Adăugarea de utilizatori externi la un grup de distribuire
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737885"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="7621a-102">Adăugarea de utilizatori externi la un grup de distribuire</span><span class="sxs-lookup"><span data-stu-id="7621a-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="7621a-103">Adăugarea unui contact extern la un grup de distribuire (DG) este un proces în două etape:</span><span class="sxs-lookup"><span data-stu-id="7621a-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="7621a-104">Creați o persoană de contact de poștă electronică pentru utilizatorul extern:</span><span class="sxs-lookup"><span data-stu-id="7621a-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="7621a-105">În centrul de administrare, accesați pagina contacte **utilizatori** > [](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="7621a-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="7621a-106">Selectați **Adăugați un contact**.</span><span class="sxs-lookup"><span data-stu-id="7621a-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="7621a-107">Tastați informațiile pentru persoana de contact și selectați **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="7621a-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="7621a-108">Adăugați contactul de poștă electronică la DG-ul dvs.:</span><span class="sxs-lookup"><span data-stu-id="7621a-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="7621a-109">În centrul de administrare, accesați > pagina[grupuri](https://admin.microsoft.com/adminportal/home#/groups) grupuri. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="7621a-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="7621a-110">Găsiți DG la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide dialogul de editare.</span><span class="sxs-lookup"><span data-stu-id="7621a-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="7621a-111">În fila **Membri** , selectați **Vizualizați toți și gestionați membrii**.</span><span class="sxs-lookup"><span data-stu-id="7621a-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="7621a-112">Selectați **Adăugați membri**.</span><span class="sxs-lookup"><span data-stu-id="7621a-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="7621a-113">Selectați contactul de poștă electronică pe care l-ați creat în pasul anterior, apoi selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="7621a-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="7621a-114">Dacă după ce urmați acești pași utilizatorii externi nu pot trimite e-mailuri la DG sau nu primesc e-mailuri de la ea, ar putea fi că DG este marcat pentru a permite numai e-mailuri de la utilizatorii interni.</span><span class="sxs-lookup"><span data-stu-id="7621a-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="7621a-115">Puteți verifica această configurație și fixați-o urmând instrucțiunile de [aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="7621a-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="7621a-116">**Notă:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "Office 365 Group" în loc de "grup de distribuire".</span><span class="sxs-lookup"><span data-stu-id="7621a-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="7621a-117">În acest caz, aveți posibilitatea să adăugați utilizatorul extern direct la grupul din Outlook.</span><span class="sxs-lookup"><span data-stu-id="7621a-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="7621a-118">Informații detaliate cu privire la Office 365 grupuri de oaspeți, precum și instrucțiuni pentru adăugarea de oaspeți externi pot fi găsite în [acest articol](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="7621a-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  