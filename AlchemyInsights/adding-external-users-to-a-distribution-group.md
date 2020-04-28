---
title: Adăugarea utilizatorilor externi la un grup de distribuire
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910944"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="8d866-102">Adăugarea utilizatorilor externi la un grup de distribuire</span><span class="sxs-lookup"><span data-stu-id="8d866-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="8d866-103">Adăugarea unui contact extern la un grup de distribuire (DG) este un proces în doi pași:</span><span class="sxs-lookup"><span data-stu-id="8d866-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="8d866-104">Crearea unei persoane de contact de poștă electronică pentru utilizatorul extern:</span><span class="sxs-lookup"><span data-stu-id="8d866-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="8d866-105">În centrul de administrare, accesați pagina[Persoane de contact](https://admin.microsoft.com/adminportal/home#/Contact) **utilizatori.** > </span><span class="sxs-lookup"><span data-stu-id="8d866-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="8d866-106">Selectați **Adăugare persoană de contact**.</span><span class="sxs-lookup"><span data-stu-id="8d866-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="8d866-107">Tastați informațiile pentru persoana de contact și selectați **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="8d866-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="8d866-108">Adăugați contactul de poștă electronică la DG:</span><span class="sxs-lookup"><span data-stu-id="8d866-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="8d866-109">În centrul de administrare, accesați pagina **Grupuri** > [grupuri.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="8d866-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="8d866-110">Găsiți DG-ul la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide dialogul de editare.</span><span class="sxs-lookup"><span data-stu-id="8d866-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="8d866-111">În fila **Membri,** selectați **Vizualizare totală și gestionare membri**.</span><span class="sxs-lookup"><span data-stu-id="8d866-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="8d866-112">Selectați **Adăugare membri**.</span><span class="sxs-lookup"><span data-stu-id="8d866-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="8d866-113">Selectați contactul de poștă electronică pe care l-ați creat la pasul anterior, apoi selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="8d866-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="8d866-114">Dacă după ce urmați acești pași, utilizatorii externi nu pot trimite e-mailuri către DG sau nu primesc e-mailuri de la acesta, este posibil ca DG să fie marcată pentru a permite numai e-mailuri de la utilizatori interni.</span><span class="sxs-lookup"><span data-stu-id="8d866-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="8d866-115">Puteți verifica această configurație și fixați-l urmând instrucțiunile [de aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="8d866-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="8d866-116">**Notã:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "Microsoft 365 group" în loc de "Grup de distribuire".</span><span class="sxs-lookup"><span data-stu-id="8d866-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="8d866-117">Dacă acesta este cazul, puteți adăuga utilizatorul extern direct la grupul din Outlook.</span><span class="sxs-lookup"><span data-stu-id="8d866-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="8d866-118">Informații detaliate despre Microsoft 365 Groups guests as well as instructions for adding external guests pot fi găsite în [acest articol](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="8d866-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  