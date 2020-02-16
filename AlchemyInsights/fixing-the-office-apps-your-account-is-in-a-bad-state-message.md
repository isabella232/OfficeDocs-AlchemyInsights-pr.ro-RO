---
title: Remedierea Aplicațiilor Office Contul dvs.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969715"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="17d72-102">Remedierea aplicațiilor Office "Contul este într-o stare proastă" eroare</span><span class="sxs-lookup"><span data-stu-id="17d72-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="17d72-103">Pentru a remedia această eroare, încercați următoarele opțiuni pe computerul afectat:</span><span class="sxs-lookup"><span data-stu-id="17d72-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="17d72-104">Deschideți o aplicație Office, selectați**Deconectare\*\*\*\*cont** > de **fișiere** > din toate conturile .</span><span class="sxs-lookup"><span data-stu-id="17d72-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="17d72-105">Conectați-vă din nou utilizând un cont de utilizator cu o licență validă.</span><span class="sxs-lookup"><span data-stu-id="17d72-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="17d72-106">Pentru informații detaliate, consultați [Conturi în Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="17d72-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="17d72-107">[Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.</span><span class="sxs-lookup"><span data-stu-id="17d72-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="17d72-108">**Notã:** Căile de registry pentru Office 2016 s-au modificat la 16.0.</span><span class="sxs-lookup"><span data-stu-id="17d72-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="17d72-109">De exemplu, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="17d72-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="17d72-110">Pe computerul afectat, setați EnableADAL = 0 utilizând următorii pași:</span><span class="sxs-lookup"><span data-stu-id="17d72-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="17d72-111">Faceți clic cu butonul din dreapta pe butonul Windows și selectați **Executare**.</span><span class="sxs-lookup"><span data-stu-id="17d72-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="17d72-112">În caseta **Deschidere,** tastați **regedit**, apoi selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="17d72-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="17d72-113">Selectați **Da** când vi se solicită să permiteți Editorului de registry să efectueze modificări pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="17d72-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="17d72-114">În Registry Editor, adăugați o valoare DWORD de EnableADAL cu o setare de 0 sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="17d72-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="17d72-115">Dacă apare eroarea în timp ce vă conectați la Office 365 utilizând Office 2013, [activați autentificarea modernă](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pentru clientul Office.</span><span class="sxs-lookup"><span data-stu-id="17d72-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="17d72-116">Pentru mai multe informații, consultați [Cum se depanează aplicațiile non-browser care nu se pot conecta la Office 365, Azure sau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="17d72-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

