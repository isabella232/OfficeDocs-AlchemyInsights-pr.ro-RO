---
title: 2681 Attack Simulator în Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759231"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="64ec4-102">Simulatorul de atac în Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="64ec4-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="64ec4-103">Vă lipsește simulatorul de atacuri?</span><span class="sxs-lookup"><span data-stu-id="64ec4-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="64ec4-104">Simulatorul de atacuri necesită **office 365 Advanced Threat Protection Plan 2 (ATP plan 2)** sau **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="64ec4-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="64ec4-105">Simulatorul de atacuri **nu** este inclus în Office 365 Advanced Threat Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3 sau orice aplicații Microsoft 365 pentru firme pentru abonamente.</span><span class="sxs-lookup"><span data-stu-id="64ec4-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="64ec4-106">Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificarea multi-factor (AMF).</span><span class="sxs-lookup"><span data-stu-id="64ec4-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="64ec4-107">Pentru mai multe informații despre cerințele pentru simulatorul de atacuri, consultați [acest subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="64ec4-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="64ec4-108">Lucruri importante de știut despre simulările de atacuri cu **parolă brută Force** :</span><span class="sxs-lookup"><span data-stu-id="64ec4-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="64ec4-109">Dacă contul țintă are AMF activat și parola a fost ghicit corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).</span><span class="sxs-lookup"><span data-stu-id="64ec4-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="64ec4-110">Fișierul parolă nu poate fi mai mare de 10 MO.</span><span class="sxs-lookup"><span data-stu-id="64ec4-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="64ec4-111">Utilizați o parolă per linie și includeți o linie necompletată (retur transport) după ultima parolă din listă.</span><span class="sxs-lookup"><span data-stu-id="64ec4-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="64ec4-112">Lucruri importante de știut despre simulările de **înșelătorie** atașate de Lance:</span><span class="sxs-lookup"><span data-stu-id="64ec4-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="64ec4-113">Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul serverului de conectare la phishing**.</span><span class="sxs-lookup"><span data-stu-id="64ec4-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="64ec4-114">Dacă un destinatar utilizează programul de [completare activare mesaj raport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pentru a raporta mesajul ca phishing, este posibil să nu primiți avertizări pentru mesaj (deoarece acesta este un atac simulat).</span><span class="sxs-lookup"><span data-stu-id="64ec4-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="64ec4-115">Rapoarte: după finalizarea atacului simulat, puteți să faceți clic pe **Detalii despre atacuri** pentru a vedea raportul.</span><span class="sxs-lookup"><span data-stu-id="64ec4-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="64ec4-116">Pentru instrucțiuni detaliate și caracteristici noi în simulatorul de atacuri, consultați [Attack Simulator în Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="64ec4-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
