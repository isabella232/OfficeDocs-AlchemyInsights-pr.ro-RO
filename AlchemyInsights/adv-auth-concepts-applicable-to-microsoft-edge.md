---
title: Concepte de autentificare complexe aplicabile în Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573528"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="34f33-102">Concepte de autentificare complexe aplicabile în Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="34f33-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="34f33-103">În continuare se află conceptele de autentificare avansată care se aplică la Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="34f33-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="34f33-104">**Autentificarea proactivă**</span><span class="sxs-lookup"><span data-stu-id="34f33-104">**Proactive Authentication**</span></span>

<span data-ttu-id="34f33-105">Atunci când activați politica [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge va încerca să autentifice proactiv utilizatori conectați prin intermediul serviciilor Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34f33-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="34f33-106">La intervale regulate, acesta va utiliza un serviciu online pentru a căuta un manifest actualizat care conține configurația care reglementează autentificarea proactivă.</span><span class="sxs-lookup"><span data-stu-id="34f33-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="34f33-107">Beneficii: autentificarea proactivă permite autentificarea la servicii cheie, cum ar fi pagina filă nouă Office.</span><span class="sxs-lookup"><span data-stu-id="34f33-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="34f33-108">De asemenea, dacă Bing este utilizat ca motor de căutare, autentificarea proactivă îmbunătățește performanța barei de adrese și ajută la generarea rezultatelor de căutare personalizate nevoilor firmei dvs.</span><span class="sxs-lookup"><span data-stu-id="34f33-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="34f33-109">**Windows Hello CredUI pentru autentificarea NTLM**</span><span class="sxs-lookup"><span data-stu-id="34f33-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="34f33-110">Dacă sign-on unic (SSO) nu este disponibil atunci când un site Web încearcă să se conecteze la utilizator prin mecanismul NTLM sau negociere, această caracteristică îi va permite utilizatorului să partajeze acreditările de sistem de operare cu site-ul web și să satisfacă provocarea de autentificare utilizând Windows Hello cred UI.</span><span class="sxs-lookup"><span data-stu-id="34f33-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="34f33-111">Acest flux de sign-on va apărea doar în Windows 10 și doar pentru utilizatorii care nu obțin SSO în timpul unei contestații NTLM sau negociere.</span><span class="sxs-lookup"><span data-stu-id="34f33-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="34f33-112">**Utilizarea parolelor salvate pentru a vă conecta automat**</span><span class="sxs-lookup"><span data-stu-id="34f33-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="34f33-113">Utilizatorii care salvează parole în Microsoft Edge pot activa conectarea automată la site-uri web în care au salvat acreditările.</span><span class="sxs-lookup"><span data-stu-id="34f33-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="34f33-114">Utilizatorii pot activa sau dezactiva această caracteristică în edge://settings/passwords și o puteți configura în politicile [Manager parole](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="34f33-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
