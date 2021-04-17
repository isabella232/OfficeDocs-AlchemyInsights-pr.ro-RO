---
title: Conectarea la Windows 10 fără a utiliza o parolă
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830558"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="cf8c1-102">Conectarea la Windows 10 fără a utiliza o parolă</span><span class="sxs-lookup"><span data-stu-id="cf8c1-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="cf8c1-103">Pentru a nu fi nevoie să tastați o parolă la pornirea Windows, vă recomandăm să utilizați una dintre opțiunile de conectare securizată Windows Hello, cum ar fi un PIN, recunoașterea feței sau amprente, dacă este disponibil.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="cf8c1-104">Dacă doriți să dezactivați conectarea securizată, consultați instrucțiunile "Conectare automată la Windows 10" de mai jos.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="cf8c1-105">**Securizarea alternativelor Windows Hello la parola contului**</span><span class="sxs-lookup"><span data-stu-id="cf8c1-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="cf8c1-106">Accesați Setări **> Conturi > Opțiuni de conectare (sau faceți** clic [aici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="cf8c1-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="cf8c1-107">Vor fi listate opțiunile disponibile de conectare.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="cf8c1-108">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="cf8c1-108">For example:</span></span>

![Opțiuni de conectare.](media/sign-in-options.png)

<span data-ttu-id="cf8c1-110">Atingeți sau faceți clic pe una dintre opțiuni pentru a o configura.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="cf8c1-111">Data viitoare când porniți sau deblocați Windows, veți putea utiliza noua opțiune în locul unei parole.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="cf8c1-112">**Conectarea automată la Windows 10**</span><span class="sxs-lookup"><span data-stu-id="cf8c1-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="cf8c1-113">**Notă:** Conectarea automată este convenabilă, dar prezintă un risc de securitate, mai ales dacă PC-ul este accesibil mai multor persoane.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="cf8c1-114">Atingeți sau faceți clic pe **butonul Start** din bara de activități.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="cf8c1-115">Tastați **netplwiz și** ajungeți la tasta Enter pentru a deschide fereastra Conturi de utilizator.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="cf8c1-116">În **Conturi de utilizator,** faceți clic pe contul la care doriți să vă conectați automat atunci când pornește Windows.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="cf8c1-117">Debifați caseta de selectare "Utilizatorii trebuie să introducă un nume de utilizator și o parolă pentru a utiliza acest computer".</span><span class="sxs-lookup"><span data-stu-id="cf8c1-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Utilizatorii trebuie să introducă o opțiune pentru numele de utilizator și parolă.](media/users-must-enter-username.png)

5. <span data-ttu-id="cf8c1-119">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-119">Click **OK**.</span></span> <span data-ttu-id="cf8c1-120">Se va solicita să introduceți și să confirmați parola pentru contul pe care l-ați selectat.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="cf8c1-121">Faceți **clic pe OK** pentru a termina.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-121">Click **OK** to finish.</span></span> <span data-ttu-id="cf8c1-122">Data viitoare când pornește Windows 10, acesta se va conecta automat la contul pe care l-ați selectat.</span><span class="sxs-lookup"><span data-stu-id="cf8c1-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
