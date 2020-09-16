---
title: Achiziție cu autoservire de PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739982"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="dbf56-102">Achiziție cu autoservire de PowerShell</span><span class="sxs-lookup"><span data-stu-id="dbf56-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="dbf56-103">Pentru a utiliza modulul PowerShell MSCommerce, trebuie să-l instalați pe un dispozitiv Windows 10 cu TLS 1,2 (permisiunile de administrator local necesare).</span><span class="sxs-lookup"><span data-stu-id="dbf56-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="dbf56-104">Importați și conectați-vă la modulul MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="dbf56-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="dbf56-105">Atunci când vi se solicită să vă conectați, va trebui să utilizați acreditările pentru rolul de administrator global sau de facturare.</span><span class="sxs-lookup"><span data-stu-id="dbf56-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="dbf56-106">Dacă nu aveți TLS 1,2, este posibil să primiți următoarea eroare atunci când încercați să obțineți sau să actualizați politica:</span><span class="sxs-lookup"><span data-stu-id="dbf56-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="dbf56-107">*ErrorMessage-conexiunea subiacentă a fost închisă: s-a produs o eroare neașteptată la trimitere*.</span><span class="sxs-lookup"><span data-stu-id="dbf56-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



