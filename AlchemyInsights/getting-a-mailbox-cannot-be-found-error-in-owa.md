---
title: 126 Eroarea Obțineți o cutie poștală nu se poate găsi în OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426674"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="dc699-102">Eroarea Obțineți o cutie poștală nu a fost găsită în Outlook pe web?</span><span class="sxs-lookup"><span data-stu-id="dc699-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="dc699-103">Dacă utilizați Outlook pe web și obțineți o cutie poștală nu **a** fost găsită din eroare, contul pe care l-ați utilizat pentru a vă conecta la Outlook pe web nu are o licență Exchange Online și, prin urmare, nu este asociată nicio cutie poștală cu contul.</span><span class="sxs-lookup"><span data-stu-id="dc699-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="dc699-104">Administratorul poate atribui o licență contului dvs. urmând acești pași:</span><span class="sxs-lookup"><span data-stu-id="dc699-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="dc699-105">Deschideți Centrul [de administrare Microsoft 365](https://portal.office.com/adminportal/home#/homepage) și  accesați Utilizatori activi sub secțiunea Utilizatori și selectați utilizatorul care vede eroarea. </span><span class="sxs-lookup"><span data-stu-id="dc699-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="dc699-106">Pe pagina de utilizator care  se deschide, accesați secțiunea  Licențe și aplicații, selectați valoarea corespunzătoare Locație și atribuiți o licență care conține Exchange Online (extindeți licența pentru a vedea detaliile).</span><span class="sxs-lookup"><span data-stu-id="dc699-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="dc699-107">Când terminați, faceți clic pe **Salvare modificări**.</span><span class="sxs-lookup"><span data-stu-id="dc699-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="dc699-108">În unele cazuri, dacă licența este atribuită deja unui cont de utilizator, eliminarea și reatriburea licenței ajută la rezolvarea problemei și asigurarea corespunzătoare a accesului la aceasta în sistem:</span><span class="sxs-lookup"><span data-stu-id="dc699-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="dc699-109">Verificați dacă abonamentele dvs. M365 Exchange Online (și altele, dacă aveți) sunt curente și nu au expirat recent.</span><span class="sxs-lookup"><span data-stu-id="dc699-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="dc699-110">După ce v-ați asigurat că abonamentul nu a expirat și i s-a atribuit o licență validă contului de utilizator, poate dura până la 24 de ore pentru ca licența să aibă acces asigurat, deci poate fi necesar să așteptați să se rezolve problema.</span><span class="sxs-lookup"><span data-stu-id="dc699-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="dc699-111">Pentru mai multe informații, [consultați Atribuirea și gestionarea licențelor.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="dc699-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>