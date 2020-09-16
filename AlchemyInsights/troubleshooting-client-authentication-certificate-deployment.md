---
title: Depanarea implementării certificatului de autentificare client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658998"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="ad5fc-102">Depanarea implementării certificatului de autentificare client</span><span class="sxs-lookup"><span data-stu-id="ad5fc-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="ad5fc-103">Profilurile de certificate client NDES/SCEP și PKCS/PFX sunt utilizate frecvent împreună cu alte tipuri de profiluri, cum ar fi WiFi, VPN și e-mail, pentru a le permite utilizatorilor să se autentifice la resurse corporative.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="ad5fc-104">Atunci când acele tipuri de profil sunt legate la un profil de certificat client depind de implementarea cu succes a acelui profil.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="ad5fc-105">Configurarea inițială a infrastructurii și configurarea asociată a profilului de certificat client necesită adesea depanare.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="ad5fc-106">Pentru un ghid pas cu pas pentru a configura cu succes conectorul NDES și instrucțiuni de depanare pentru a izola problemele cu implementarea certificatelor, consultați:</span><span class="sxs-lookup"><span data-stu-id="ad5fc-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="ad5fc-107">Configurarea infrastructurii pentru a accepta SCEP cu Intune</span><span class="sxs-lookup"><span data-stu-id="ad5fc-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="ad5fc-108">Prezentare generală pentru depanarea profilurilor de certificat SCEP cu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ad5fc-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="ad5fc-109">Utilizați Scripturile PowerShell la care se face referire pentru a vă verifica configurația.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="ad5fc-110">Pentru mai multe informații, consultați [scripturi de verificare a conectorului de certificat Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="ad5fc-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="ad5fc-111">**Alte probleme comune**</span><span class="sxs-lookup"><span data-stu-id="ad5fc-111">**Other common issues**</span></span>

<span data-ttu-id="ad5fc-112">**Atunci când încerc să instalez conectorul de certificat Intune pe serverul de conector NDES, primesc mesajul "parola din solicitarea de certificat nu poate fi verificată. Este posibil să fi fost utilizat deja. Obțineți o parolă nouă pentru a o trimite cu această solicitare. "**</span><span class="sxs-lookup"><span data-stu-id="ad5fc-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="ad5fc-113">Acest mesaj înseamnă că trebuie să ruleze instalarea conectorului de certificat ca administrator.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="ad5fc-114">În unele medii, serverele în care rulează certificatul Intune trebuie să utilizeze un server proxy pentru a se conecta la Intune, astfel încât conectorul de certificat să utilizeze un proxy.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="ad5fc-115">În unele împrejurări, conectorul NDES ignoră setările proxy configurate și poate fi necesar să configurați setările proxy în timp ce se execută în contextul de securitate al LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="ad5fc-116">Soluția este să ruleze Internet Explorer ca sistem și să configurați un proxy în IE.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="ad5fc-117">După o repornire a serviciului conector Intune, conectorul NDES se conectează la Intune.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="ad5fc-118">**Dispozitivele de utilizator nu mai primesc certificatele SCEP de la NDES.**</span><span class="sxs-lookup"><span data-stu-id="ad5fc-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="ad5fc-119">Este posibil ca certificatul de autentificare client emis la serverul NDES și specificat în timpul instalării conectorului NDES să fie expirat sau lipsește.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="ad5fc-120">Pentru a rezolva:</span><span class="sxs-lookup"><span data-stu-id="ad5fc-120">To resolve:</span></span> 
 
1. <span data-ttu-id="ad5fc-121">Dezinstalați conectorul NDES.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="ad5fc-122">Utilizați aceste detalii pentru a solicita o nouă autentificare de client sau un certificat de autentificare de server:</span><span class="sxs-lookup"><span data-stu-id="ad5fc-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="ad5fc-123">Nume subiect: CN = FQDN extern</span><span class="sxs-lookup"><span data-stu-id="ad5fc-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="ad5fc-124">Nume alternativ subiect (ambele sunt necesare): DNS = externe FQDN, DNS = Internal FQDN</span><span class="sxs-lookup"><span data-stu-id="ad5fc-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="ad5fc-125">Reinstalați conectorul NDES cu noul certificat.</span><span class="sxs-lookup"><span data-stu-id="ad5fc-125">Reinstall the NDES connector with the new certificate.</span></span>