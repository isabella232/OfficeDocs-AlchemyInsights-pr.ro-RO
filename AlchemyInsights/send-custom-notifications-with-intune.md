---
title: Trimiteți notificări personalizate cu Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886869"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="9566d-102">să trimiteți notificări personalizate utilizatorilor de dispozitive iOS și Android gestionate</span><span class="sxs-lookup"><span data-stu-id="9566d-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="9566d-103">Notificările particularizate pentru Intune sunt procesate de aplicația portal de companie pe dispozitivul unui utilizator.</span><span class="sxs-lookup"><span data-stu-id="9566d-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="9566d-104">Aplicația apoi creează notificarea Push pe acel dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="9566d-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="9566d-105">Următoarele sunt premise pentru dispozitiv pentru a accepta primirea notificărilor particularizate și pentru ca aplicația să creeze apoi notificarea Push:</span><span class="sxs-lookup"><span data-stu-id="9566d-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="9566d-106">Dispozitivul trebuie să aibă instalată aplicația portal de companie.</span><span class="sxs-lookup"><span data-stu-id="9566d-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="9566d-107">Dispozitivul trebuie să permită aplicației portal companie să trimită notificări Push.</span><span class="sxs-lookup"><span data-stu-id="9566d-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="9566d-108">Când aplicația este instalată sau actualizată, va solicita utilizatorului să permită notificări.</span><span class="sxs-lookup"><span data-stu-id="9566d-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="9566d-109">Dispozitivele Android trebuie să aibă instalat serviciile Google Play.</span><span class="sxs-lookup"><span data-stu-id="9566d-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="9566d-110">Dispozitivul trebuie să fie înscris cu Intune.</span><span class="sxs-lookup"><span data-stu-id="9566d-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="9566d-111">Pentru mai multe informații, inclusiv să trimiteți un mesaj, consultați [documentația caracteristică](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="9566d-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
