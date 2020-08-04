---
title: Depanarea implementării certificatului de autentificare client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555301"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="854e3-102">Depanarea implementării certificatului de autentificare client</span><span class="sxs-lookup"><span data-stu-id="854e3-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="854e3-103">Intune NDES/SCEP și PKCS/PFX Profilurile de certificate client sunt utilizate în mod obișnuit împreună cu alte tipuri de profiluri, ar fi Wifi, VPN și e-mail pentru a permite utilizatorilor să se autentifice la resursele companiei.</span><span class="sxs-lookup"><span data-stu-id="854e3-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="854e3-104">Atunci când aceste tipuri de profil sunt legate la un profil de certificat de client depind de implementarea cu succes a acelui profil.</span><span class="sxs-lookup"><span data-stu-id="854e3-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="854e3-105">Configurarea inițială a infrastructurii și configurarea asociată a profilului certificatului client necesită adesea depanare.</span><span class="sxs-lookup"><span data-stu-id="854e3-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="854e3-106">Pentru un ghid pas cu pas pentru configurarea cu succes a conectorului NDES și instrucțiuni de depanare pentru a izola problemele legate de implementarea certificatului, consultați:</span><span class="sxs-lookup"><span data-stu-id="854e3-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="854e3-107">Configurarea infrastructurii pentru a accepta SCEP cu Intune</span><span class="sxs-lookup"><span data-stu-id="854e3-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="854e3-108">Prezentare generală pentru depanarea profilurilor de certificate SCEP cu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="854e3-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="854e3-109">Utilizați scripturile powershell la care se face referire pentru a vă ajuta să verificați configurația.</span><span class="sxs-lookup"><span data-stu-id="854e3-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="854e3-110">Pentru mai multe informații, consultați [Scripturile de verificare a conectorilor de certificate Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="854e3-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="854e3-111">**Alte probleme comune**</span><span class="sxs-lookup"><span data-stu-id="854e3-111">**Other common issues**</span></span>

<span data-ttu-id="854e3-112">**Când încerc să instalez conectorul de certificat Intune pe serverul conector NDES, primesc mesajul, "Parola din solicitarea de certificat nu poate fi verificată. Este posibil să fi fost deja folosit. Obțineți o parolă nouă de trimis cu această solicitare."**</span><span class="sxs-lookup"><span data-stu-id="854e3-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="854e3-113">Acest mesaj înseamnă că trebuie să executați instalarea conectorului de certificat ca administrator.</span><span class="sxs-lookup"><span data-stu-id="854e3-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="854e3-114">În unele medii, serverele unde se execută Certificatul Intune trebuie să utilizeze un server proxy pentru a se conecta la Intune, astfel încât Conectorul de certificat trebuie să utilizeze un proxy.</span><span class="sxs-lookup"><span data-stu-id="854e3-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="854e3-115">În unele circumstanțe, Conectorul NDES ignoră setările proxy configurate și poate fi necesar să configurați setările proxy în timp ce se execută în contextul de securitate al LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="854e3-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="854e3-116">Soluția este să executați Internet Explorer ca SISTEM și să configurați un proxy în IE.</span><span class="sxs-lookup"><span data-stu-id="854e3-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="854e3-117">După repornirea serviciului Intune Connector, conectorul NDES se conectează la Intune.</span><span class="sxs-lookup"><span data-stu-id="854e3-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="854e3-118">**Dispozitivele utilizator nu mai primesc certificate SCEP de la NDES.**</span><span class="sxs-lookup"><span data-stu-id="854e3-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="854e3-119">Este posibil ca certificatul de autentificare client emis pe serverul NDES și specificat în timpul instalării conectorului NDES, să fi expirat sau să lipsească.</span><span class="sxs-lookup"><span data-stu-id="854e3-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="854e3-120">Pentru a rezolva:</span><span class="sxs-lookup"><span data-stu-id="854e3-120">To resolve:</span></span> 
 
1. <span data-ttu-id="854e3-121">Dezinstalați conectorul NDES.</span><span class="sxs-lookup"><span data-stu-id="854e3-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="854e3-122">Utilizați aceste detalii pentru a solicita un nou certificat de autentificare client sau de autentificare server:</span><span class="sxs-lookup"><span data-stu-id="854e3-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="854e3-123">Nume subiect: CN=fqdn extern</span><span class="sxs-lookup"><span data-stu-id="854e3-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="854e3-124">Nume alternativ subiect (ambele sunt necesare): DNS=fqdn extern, DNS=fqdn intern</span><span class="sxs-lookup"><span data-stu-id="854e3-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="854e3-125">Reinstalați conectorul NDES cu noul certificat.</span><span class="sxs-lookup"><span data-stu-id="854e3-125">Reinstall the NDES connector with the new certificate.</span></span>