---
title: 2681 Attack Simulator în Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506750"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="cda7b-102">Attack Simulator în Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cda7b-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="cda7b-103">Îți lipsește Simulatorul de atac?</span><span class="sxs-lookup"><span data-stu-id="cda7b-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="cda7b-104">Attack Simulator necesită **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** sau **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="cda7b-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="cda7b-105">Attack Simulator **nu** este inclus în Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 sau orice Microsoft 365 Apps for business abonamente.</span><span class="sxs-lookup"><span data-stu-id="cda7b-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="cda7b-106">Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificare multi-factor (MAE).</span><span class="sxs-lookup"><span data-stu-id="cda7b-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="cda7b-107">Pentru mai multe informații despre cerințele Attack Simulator, consultați [acest subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="cda7b-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="cda7b-108">Lucruri importante de știut despre simulările de atac **brute force password:**</span><span class="sxs-lookup"><span data-stu-id="cda7b-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="cda7b-109">Dacă contul țintă are AMF activat și parola a fost ghicit corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).</span><span class="sxs-lookup"><span data-stu-id="cda7b-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="cda7b-110">Fișierul parolă nu poate fi mai mare de 10 MO.</span><span class="sxs-lookup"><span data-stu-id="cda7b-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="cda7b-111">Utilizați o parolă pe linie și includeți o linie necompletată (retur de transport) după ultima parolă din listă.</span><span class="sxs-lookup"><span data-stu-id="cda7b-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="cda7b-112">Lucruri importante de știut despre simulările de **atașare a sperei phishing:**</span><span class="sxs-lookup"><span data-stu-id="cda7b-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="cda7b-113">După proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul serverului de conectare phishing**.</span><span class="sxs-lookup"><span data-stu-id="cda7b-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="cda7b-114">Dacă un destinatar utilizează [programul de completare Activare mesaj raport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pentru a raporta mesajul ca phishing, este posibil să nu primiți alerte pentru mesaj (deoarece acesta este un atac simulat).</span><span class="sxs-lookup"><span data-stu-id="cda7b-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="cda7b-115">Rapoarte: După terminarea atacului simulat, puteți face clic pe **Detalii atac** pentru a vedea raportul.</span><span class="sxs-lookup"><span data-stu-id="cda7b-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="cda7b-116">Pentru instrucțiuni detaliate și caracteristici noi în Attack Simulator, consultați [Attack Simulator în Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="cda7b-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
