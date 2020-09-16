---
title: Conectarea la Windows 10 fără a utiliza o parolă
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719965"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="4cf47-102">Conectarea la Windows 10 fără a utiliza o parolă</span><span class="sxs-lookup"><span data-stu-id="4cf47-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="4cf47-103">Pentru a evita să tastați o parolă la pornirea Windows, vă recomandăm să utilizați una dintre opțiunile de conectare Windows Hello Secure, cum ar fi un cod PIN, o recunoaștere a feței sau o amprentă, dacă este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="4cf47-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="4cf47-104">Dacă doriți într-adevăr să dezactivați conectarea securizată, consultați instrucțiunile "conectați-vă automat la Windows 10" de mai jos.</span><span class="sxs-lookup"><span data-stu-id="4cf47-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="4cf47-105">**Securizați alternativele Windows Hello la parola contului**</span><span class="sxs-lookup"><span data-stu-id="4cf47-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="4cf47-106">Accesați **setări > conturi > opțiuni de conectare** (sau faceți clic [aici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="4cf47-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="4cf47-107">Opțiunile de conectare disponibile vor fi listate.</span><span class="sxs-lookup"><span data-stu-id="4cf47-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="4cf47-108">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="4cf47-108">For example:</span></span>

![Opțiuni de conectare.](media/sign-in-options.png)

<span data-ttu-id="4cf47-110">Atingeți sau faceți clic pe una dintre opțiuni pentru a o configura.</span><span class="sxs-lookup"><span data-stu-id="4cf47-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="4cf47-111">Data viitoare când porniți sau deblocați Windows, veți putea utiliza opțiunea nouă în locul unei parole.</span><span class="sxs-lookup"><span data-stu-id="4cf47-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="4cf47-112">**Conectarea automată la Windows 10**</span><span class="sxs-lookup"><span data-stu-id="4cf47-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="4cf47-113">**Notă**: Conectarea automată este convenabilă, dar prezintă un risc de securitate, mai ales dacă PC-ul este accesibil de mai multe persoane.</span><span class="sxs-lookup"><span data-stu-id="4cf47-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="4cf47-114">Atingeți sau faceți clic pe butonul **Start** în bara de activități.</span><span class="sxs-lookup"><span data-stu-id="4cf47-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="4cf47-115">Tastați **netplwiz** și apăsați tasta Enter pentru a deschide fereastra conturi utilizator.</span><span class="sxs-lookup"><span data-stu-id="4cf47-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="4cf47-116">În **conturile de utilizator**, faceți clic pe contul la care doriți să vă conectați automat atunci când pornește Windows.</span><span class="sxs-lookup"><span data-stu-id="4cf47-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="4cf47-117">Debifați caseta de selectare "utilizatorii trebuie să introducă un nume de utilizator și o parolă pentru a utiliza acest computer".</span><span class="sxs-lookup"><span data-stu-id="4cf47-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Utilizatorii trebuie să introducă o opțiune de nume de utilizator și parolă.](media/users-must-enter-username.png)

5. <span data-ttu-id="4cf47-119">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="4cf47-119">Click **OK**.</span></span> <span data-ttu-id="4cf47-120">Vi se va solicita să introduceți și să confirmați parola pentru contul pe care l-ați selectat.</span><span class="sxs-lookup"><span data-stu-id="4cf47-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="4cf47-121">Faceți clic pe **OK** pentru a termina.</span><span class="sxs-lookup"><span data-stu-id="4cf47-121">Click **OK** to finish.</span></span> <span data-ttu-id="4cf47-122">Data viitoare când pornește Windows 10, acesta se va conecta automat la contul pe care l-ați selectat.</span><span class="sxs-lookup"><span data-stu-id="4cf47-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
