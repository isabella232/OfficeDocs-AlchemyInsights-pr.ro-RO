---
title: Activați Rescriere parole în Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814024"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="0b751-102">Activați Rescriere parole în Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="0b751-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="0b751-103">Pentru a activa resetarea opțiunii Rescriere parole, mai întâi activați opțiunea Rescriere parole în Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="0b751-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="0b751-104">Din serverul dvs. Azure AD Connect, completați următorii pași:</span><span class="sxs-lookup"><span data-stu-id="0b751-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="0b751-105">Conectați-vă la serverul dvs. Azure AD Connect și demarați expertul de configurare **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="0b751-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="0b751-106">Pe pagina **Bun venit**, faceți clic pe **Configurare**.</span><span class="sxs-lookup"><span data-stu-id="0b751-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="0b751-107">Pe pagina **Activități suplimentare**, selectați **Particularizare opțiuni de sincronizare**, și apoi faceți clic pe **Următorul**.</span><span class="sxs-lookup"><span data-stu-id="0b751-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="0b751-108">Pe pagina **Conectare la Azure AD**, introduceți o acreditare administrator global pentru locatarul Azure și apoi faceți clic pe **Următorul**.</span><span class="sxs-lookup"><span data-stu-id="0b751-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="0b751-109">În directoarele **Conectare** și paginile de filtrare **Domain/OU** faceți clic pe **Următorul**.</span><span class="sxs-lookup"><span data-stu-id="0b751-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="0b751-110">Pe pagina **Caracteristici opționale**, selectați caseta de lângă **Rescriere parole** și faceți clic pe **Următorul**.</span><span class="sxs-lookup"><span data-stu-id="0b751-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="0b751-111">Pe pagina **Gata de configurat**, faceți clic pe **Configurare** și așteptați terminarea procesului.</span><span class="sxs-lookup"><span data-stu-id="0b751-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="0b751-112">Atunci când vedeți că s-a terminat configurarea, faceți clic pe **Ieșire**.</span><span class="sxs-lookup"><span data-stu-id="0b751-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="0b751-113">Cu Rescrierea parolei activată în Azure AD Connect, configurați Azure AD SSPR pentru rescrierea parolei.</span><span class="sxs-lookup"><span data-stu-id="0b751-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="0b751-114">Pentru a activa rescrierea parolei în SSPR, completați următorii pași:</span><span class="sxs-lookup"><span data-stu-id="0b751-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="0b751-115">Conectați-vă la portalul Azure utilizând un cont de administrator global.</span><span class="sxs-lookup"><span data-stu-id="0b751-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="0b751-116">Căutați și selectați **Azure Active Directory**, faceți clic pe **Resetare parolă**, apoi faceți clic pe **Integrare locală**.</span><span class="sxs-lookup"><span data-stu-id="0b751-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="0b751-117">Setați opțiunea **Rescriere parole pentru directorul local?** la **Da**.</span><span class="sxs-lookup"><span data-stu-id="0b751-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="0b751-118">Setați opțiunea **Permiteți utilizatorilor să deblocheze conturile fără a-și reseta parolele?** la **Da**.</span><span class="sxs-lookup"><span data-stu-id="0b751-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="0b751-119">Atunci când sunteți pregătit, faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="0b751-119">When ready, click **Save**.</span></span>

<span data-ttu-id="0b751-120">Pentru mai multe informații, vedeți [Activarea rescrierii parolelor în Azure Active Directory într-un domeniu local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="0b751-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="0b751-121">Atunci când un administrator resetează parola unui utilizator în portalul Azure, dacă acel utilizator este federativ sau hash-ul parolei este sincronizat, parola este scrisă din nou la local.</span><span class="sxs-lookup"><span data-stu-id="0b751-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="0b751-122">Această funcționalitate necesită licență Azure Premium (P1 sau P2) și nu este acceptată momentan în portalul de administrare Office.</span><span class="sxs-lookup"><span data-stu-id="0b751-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
