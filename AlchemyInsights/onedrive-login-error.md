---
title: Eroare de conectare la OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982543"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="332fd-102">Eroare de conectare la OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="332fd-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="332fd-103">Dacă primiți o eroare "AADSTS50011: adresa URL de răspuns specificată în solicitare nu se potrivește cu răspunsul" atunci când vă conectați la aplicația OneDrive, verificați următoarele:</span><span class="sxs-lookup"><span data-stu-id="332fd-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="332fd-104">Versiunea dumneavoastră OneDrive trebuie să fie egală cu sau mai mare decât versiunea 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="332fd-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="332fd-105">Pentru a vă verifica versiunea, faceți clic pe pictograma OneDrive albastră din zona de notificare, selectați **ajutor & setări > setări >**.</span><span class="sxs-lookup"><span data-stu-id="332fd-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="332fd-106">Este posibil ca rețeaua să blocheze traficul către **g.live.com** și **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="332fd-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="332fd-107">Dacă traficul este blocat, OneDrive nu se poate actualiza singur.</span><span class="sxs-lookup"><span data-stu-id="332fd-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="332fd-108">Lucrați cu administratorul de rețea pentru a vă asigura că aveți acces la acele URL-uri.</span><span class="sxs-lookup"><span data-stu-id="332fd-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="332fd-109">[Aceste puncte finale](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) ar trebui să fie accesibile pentru clienții care utilizează Microsoft 365 planuri.</span><span class="sxs-lookup"><span data-stu-id="332fd-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="332fd-110">Dacă trebuie să obțineți manual o versiune curentă de OneDrive, vizitați [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="332fd-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
