---
title: Certificatul de împingere Apple MDM nu a fost configurat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440013"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="30727-102">Certificatul de împingere Apple MDM nu a fost configurat</span><span class="sxs-lookup"><span data-stu-id="30727-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="30727-103">Un certificat apple MDM Push Certificate (cunoscut și ca certificat APNS (Apple Push Notification Service) nu a fost configurat pentru abonamentul dvs.</span><span class="sxs-lookup"><span data-stu-id="30727-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="30727-104">Fără un certificat apple MDM push configurat, nu poți să te înscrii și să gestionezi dispozitivele iOS și Mac OS.</span><span class="sxs-lookup"><span data-stu-id="30727-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="30727-105">După ce adăugați certificatul la Intune, utilizatorii pot instala aplicația Portal companie pentru a-și înscrie dispozitivele iOS.</span><span class="sxs-lookup"><span data-stu-id="30727-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="30727-106">Selectați **"Sunt de acord."**</span><span class="sxs-lookup"><span data-stu-id="30727-106">Select **"I agree."**</span></span> <span data-ttu-id="30727-107">pentru a acorda Microsoft permisiunea de a trimite date către Apple.</span><span class="sxs-lookup"><span data-stu-id="30727-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="30727-108">Selectați **Descărcați CSR** solicitarea de semnare a certificatului Intune necesară pentru a crea un certificat de împingere Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="30727-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="30727-109">Fișierul este utilizat pentru a solicita un certificat de relație de încredere de la Portalul de certificate de împingere Apple.</span><span class="sxs-lookup"><span data-stu-id="30727-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="30727-110">Selectează **Creează certificatul de împingere MDM** pentru a accesa portalul apple push certificates.</span><span class="sxs-lookup"><span data-stu-id="30727-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="30727-111">Conectați-vă cu ID-ul Apple al companiei, apoi selectați **Creare certificat**.</span><span class="sxs-lookup"><span data-stu-id="30727-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="30727-112">Selectați **Alegere fișier**, răsfoiți la fișierul de solicitare a semnării certificatului, apoi **selectați Încărcare**.</span><span class="sxs-lookup"><span data-stu-id="30727-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="30727-113">Pe pagina Confirmare, alegeți **Descărcare** pentru a descărca fișierul certificat (.pem) și a salva fișierul local.</span><span class="sxs-lookup"><span data-stu-id="30727-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="30727-114">**Notă:** Certificatul este asociat cu ID-ul Apple utilizat pentru a-l crea.</span><span class="sxs-lookup"><span data-stu-id="30727-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="30727-115">Ca o bună practică, utilizați un ID Apple al companiei pentru activități de gestionare și asigurați-vă că cutia poștală este monitorizată de mai multe persoane sau utilizând o listă de distribuire.</span><span class="sxs-lookup"><span data-stu-id="30727-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="30727-116">Nu folosiți niciodată un ID Apple personal.</span><span class="sxs-lookup"><span data-stu-id="30727-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="30727-117">Folosește același ID Apple pentru a reînnoi Certificatul de împingere Apple la fiecare 12 luni.</span><span class="sxs-lookup"><span data-stu-id="30727-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="30727-118">Introduceți ID-ul Apple utilizat pentru a crea certificatul de împingere Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="30727-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="30727-119">Înregistrați acest ID ca memento pentru momentul în care trebuie să reînnoiți certificatul.</span><span class="sxs-lookup"><span data-stu-id="30727-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="30727-120">Accesați fișierul certificat (.pem), alegeți **Deschidere**, apoi alegeți **Încărcare**.</span><span class="sxs-lookup"><span data-stu-id="30727-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="30727-121">Cu certificatul push, Intune se poate înscrie și gestiona dispozitivele Apple.</span><span class="sxs-lookup"><span data-stu-id="30727-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>