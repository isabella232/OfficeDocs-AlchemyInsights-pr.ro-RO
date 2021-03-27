---
title: Concepte de autentificare avansate care se aplică la Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398597"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="10207-102">Concepte de autentificare avansate care se aplică la Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="10207-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="10207-103">În cele ce urmează conceptele de autentificare avansate care se aplică la Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="10207-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="10207-104">**Autentificare proactivă**</span><span class="sxs-lookup"><span data-stu-id="10207-104">**Proactive Authentication**</span></span>

<span data-ttu-id="10207-105">Atunci când activați [politica ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge va încerca să autentifice proactiv utilizatorii autentificați prin intermediul serviciilor Microsoft.</span><span class="sxs-lookup"><span data-stu-id="10207-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="10207-106">La intervale regulate, acesta va utiliza un serviciu online pentru a căuta un manifest actualizat care conține configurația care guvernează autentificarea Proactivă.</span><span class="sxs-lookup"><span data-stu-id="10207-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="10207-107">Avantaje: Autentificarea proactivă permite autentificarea la servicii cheie, cum ar fi pagina Filă nouă Office.</span><span class="sxs-lookup"><span data-stu-id="10207-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="10207-108">De asemenea, dacă Bing este utilizat ca motor de căutare, Autentificarea proactivă îmbunătățește performanța barei de adrese și vă ajută să generați rezultate de căutare personalizate pentru necesitățile firmei dvs.</span><span class="sxs-lookup"><span data-stu-id="10207-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="10207-109">**Windows Hello CredUI pentru autentificare NTLM**</span><span class="sxs-lookup"><span data-stu-id="10207-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="10207-110">Dacă caracteristica sign-on unic (SSO) nu este disponibilă atunci când un site web încearcă să se conecteze la utilizator prin intermediul mecanismului NTLM sau Negociați, această caracteristică va permite utilizatorului să partajeze acreditările sistemului de operare cu site-ul web și să îndeplinească provocarea autentificării utilizând interfața utilizator Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="10207-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="10207-111">Acest flux de sign-on va apărea doar în Windows 10 și doar pentru utilizatorii care nu primesc SSO în timpul unei proceduri NTLM sau a unei provocări de negociare.</span><span class="sxs-lookup"><span data-stu-id="10207-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="10207-112">**Utilizați parole salvate pentru a vă conecta automat**</span><span class="sxs-lookup"><span data-stu-id="10207-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="10207-113">Utilizatorii care salvează parole în Microsoft Edge pot activa conectarea automată la site-urile web unde au salvat acreditări.</span><span class="sxs-lookup"><span data-stu-id="10207-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="10207-114">Utilizatorii pot activa sau dezactiva această caracteristică edge://settings/passwords și o puteți configura în politicile [managerului](https://go.microsoft.com/fwlink/?linkid=2134622) de parole.</span><span class="sxs-lookup"><span data-stu-id="10207-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
