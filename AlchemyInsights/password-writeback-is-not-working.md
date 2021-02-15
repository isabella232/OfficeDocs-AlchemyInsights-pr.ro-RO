---
title: Writeback parolelor nu funcționează
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243520"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="4a5f7-102">Writeback parolelor nu funcționează</span><span class="sxs-lookup"><span data-stu-id="4a5f7-102">Password Writeback is not working</span></span>

<span data-ttu-id="4a5f7-103">**Am probleme cu configurarea parolei writeback**</span><span class="sxs-lookup"><span data-stu-id="4a5f7-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="4a5f7-104">Writeback parolelor este o caracteristică premium.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="4a5f7-105">Asigurați-vă că înțelegeți cerințele de licențiere:</span><span class="sxs-lookup"><span data-stu-id="4a5f7-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="4a5f7-106">Trebuie să aveți cel puțin o licență atribuită în organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="4a5f7-107">**Utilizatori Cloud Only** -orice Office 365 (O365) a plătit SKU sau Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="4a5f7-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="4a5f7-108">**Utilizatori cloud și/sau locali** -Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="4a5f7-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="4a5f7-109">Pentru a afla mai multe despre cerințele de licențiere, consultați [cerințe de licențiere pentru resetarea parolei cu autoservire AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="4a5f7-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="4a5f7-110">Aveți cel puțin un cont de administrator și un cont de utilizator test cu una dintre licențele corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="4a5f7-111">Trebuie să conectați Azure AD Connect la emulatorul controlerului de domeniu principal pentru writeback parolei pentru a funcționa.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="4a5f7-112">Puteți configura Azure AD Connect pentru a utiliza un controler de domeniu principal, făcând clic dreapta pe **proprietățile** conectorului de sincronizare Active Directory, apoi selectând **configurare partiții directoare**.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="4a5f7-113">De acolo, căutați secțiunea **Setări conexiune controler de domeniu** și bifați caseta intitulată **Utilizați doar controlerele de domeniu preferate**.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="4a5f7-114">Dacă DC-ul preferat nu este un emulator PDC, Azure AD Connect va ajunge în continuare la PDC pentru password writeback.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="4a5f7-115">Resetarea parolei a fost configurată și activată în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="4a5f7-116">Pentru mai multe informații, consultați [Activarea utilizatorilor pentru a reseta parolele AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="4a5f7-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="4a5f7-117">Asigurați-vă că contul de administrator utilizat pentru a activa parola writeback este un cont de administrator Cloud (creat în Azure AD nu AD local)</span><span class="sxs-lookup"><span data-stu-id="4a5f7-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="4a5f7-118">Aveți o implementare reclamă locală unică sau mai multe păduri care execută Windows Server 2008 R2, Windows Server 2012 sau Windows Server 2012 R2 cu cele mai recente pachete Service Pack instalate</span><span class="sxs-lookup"><span data-stu-id="4a5f7-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="4a5f7-119">Ați instalat instrumentul Azure AD Connect și ați pregătit mediul publicitar pentru sincronizarea cu Cloud.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="4a5f7-120">Înainte să testați parola writeback, asigurați-vă că ați finalizat pentru prima dată un import complet și sincronizare completă atât din AD, cât și din Azure AD în Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4a5f7-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="4a5f7-121">Pentru a afla mai multe, consultați Cum se face o [Sincronizare completă și importul integral în AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="4a5f7-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="4a5f7-122">**Am o problemă cu conectivitatea writeback prin parolă**</span><span class="sxs-lookup"><span data-stu-id="4a5f7-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="4a5f7-123">Descărcarea și activarea celei mai recente versiuni de [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="4a5f7-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="4a5f7-124">Configurarea paravanului de protecție: instrumentul Azure AD Connect (1.1.443 și above) va avea nevoie de acces **https de ieșire** la:</span><span class="sxs-lookup"><span data-stu-id="4a5f7-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="4a5f7-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4a5f7-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="4a5f7-126">ServiceBus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="4a5f7-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="4a5f7-127">Permiteți conexiunilor Idle să persiste cel puțin 2-3 de minute</span><span class="sxs-lookup"><span data-stu-id="4a5f7-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="4a5f7-128">**Am în continuare probleme cu parola writeback**</span><span class="sxs-lookup"><span data-stu-id="4a5f7-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="4a5f7-129">Dacă încă întâmpinați dificultăți, încercați să dezactivați și să activați din nou serviciul de writeback a parolei în instrumentul Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="4a5f7-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="4a5f7-130">Pentru a afla mai multe, consultați Cum să [Dezactivați și să activați din nou parola writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="4a5f7-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
