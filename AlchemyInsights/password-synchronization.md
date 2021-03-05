---
title: Sincronizare parole
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483081"
---
# <a name="password-synchronization"></a><span data-ttu-id="1b6ec-102">Sincronizare parole</span><span class="sxs-lookup"><span data-stu-id="1b6ec-102">Password synchronization</span></span>

<span data-ttu-id="1b6ec-103">**Sincronizarea codului hash pentru parole nu funcționează deloc**</span><span class="sxs-lookup"><span data-stu-id="1b6ec-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="1b6ec-104">Unele probleme uzuale pe care le întâmpină clienții atunci când sincronizarea hash a parolelor nu funcționează sunt:</span><span class="sxs-lookup"><span data-stu-id="1b6ec-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="1b6ec-105">Contul Active Directory utilizat de Azure AD Connect pentru a comunica cu Active Directory local nu îi este permis să **reproducă modificări de Director** și să **reproducă modificările directorului toate** permisiunile, necesare pentru sincronizarea parolelor-trebuie să remediați acest lucru prin acordarea acestor permisiuni la contul Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="1b6ec-106">Sincronizarea codului hash pentru parole este dezactivată după ce un administrator a modificat metoda de Sign-In utilizator de la **sincronizarea parolelor** la o altă opțiune, cum ar fi **Federation cu AD FS** din Azure AD Connect Wizard-puteți remedia acest lucru prin reactivarea caracteristicii de **sincronizare a parolei hash** în Expertul Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="1b6ec-107">Problemă de conectivitate cu Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="1b6ec-108">De exemplu, unele controlere de domeniu nu sunt accesibile prin Azure AD Connect sau [porturile necesare](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) sunt blocate de Paravanul de protecție-trebuie să remediați această problemă, asigurându-vă că conectivitatea dintre serverul Azure AD Connect și Active Directory local funcționează corect.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="1b6ec-109">Serverul Azure AD Connect se află în prezent în modul de așteptare, ceea ce va determina ca serverul să nu poată face codul hash pentru parole-pentru a depana problema, urmați pașii descriși în secțiunea [Depanarea sincronizării parolelor cu sincronizarea AZURE AD Connect-nu se sincronizează parole](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="1b6ec-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="1b6ec-110">**Sincronizarea hash a parolei nu funcționează pentru unii dintre utilizatorii mei**</span><span class="sxs-lookup"><span data-stu-id="1b6ec-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="1b6ec-111">Dacă ați observat că parola hash nu se sincronizează pentru un utilizator, utilizați activitatea de **Depanare** din Azure AD Connect pentru a investiga și a rezolva problema.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="1b6ec-112">Efectuați următoarele activități:</span><span class="sxs-lookup"><span data-stu-id="1b6ec-112">Perform the following tasks:</span></span>

    <span data-ttu-id="1b6ec-113">un.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-113">a.</span></span> [<span data-ttu-id="1b6ec-114">Rularea activității de depanare în expert</span><span class="sxs-lookup"><span data-stu-id="1b6ec-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="1b6ec-115">b.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-115">b.</span></span> [<span data-ttu-id="1b6ec-116">Utilizați cmdletul depanare pentru a investiga problema de sincronizare a parolelor hash pentru o utilizare specifică</span><span class="sxs-lookup"><span data-stu-id="1b6ec-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="1b6ec-117">Obiectul de utilizator Active Directory local este activat pentru **utilizator trebuie să modifice parola la următoarea** opțiune de conectare.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="1b6ec-118">Atunci când această opțiune este activată, utilizatorului i se atribuie o parolă temporară și vi se va solicita să modificați parola la următorul logon.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="1b6ec-119">Azure AD Connect nu sincronizează parolele temporare cu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="1b6ec-120">Pentru a rezolva problema de mai sus, efectuați oricare dintre următoarele activități:</span><span class="sxs-lookup"><span data-stu-id="1b6ec-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="1b6ec-121">Solicitați utilizatorului să se conecteze la o aplicație locală (de exemplu, desktop Windows) și să modifice parola.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="1b6ec-122">Noua parolă va fi sincronizată cu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="1b6ec-123">Depuneți un administrator să actualizeze parola utilizatorului fără a permite **utilizatorului opțiunea să modifice parola la următorul log on** și să partajeze noua parolă cu utilizatorul.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="1b6ec-124">Obiectul de utilizator Active Directory local **nu este configurat corect** pentru sincronizarea obiectelor sau sincronizarea parolelor.</span><span class="sxs-lookup"><span data-stu-id="1b6ec-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="1b6ec-125">Pentru a depana această problemă, urmați pașii descriși în [sincronizarea hash a parolei cu sincronizarea AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="1b6ec-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







