---
title: Trimiterea de notificări particularizate cu Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720658"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="f2601-102">Cum să trimiteți notificări particularizate utilizatorilor de dispozitive iOS și Android gestionate</span><span class="sxs-lookup"><span data-stu-id="f2601-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="f2601-103">Notificările particularizate pentru Intune sunt prelucrate de aplicația portal a firmei pe dispozitivul unui utilizator.</span><span class="sxs-lookup"><span data-stu-id="f2601-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="f2601-104">Aplicația creează apoi notificarea Push pe acel dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="f2601-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="f2601-105">Următoarele sunt cerințe preliminare pentru dispozitive pentru a accepta primirea notificărilor particularizate și pentru ca aplicația să creeze apoi notificarea Push:</span><span class="sxs-lookup"><span data-stu-id="f2601-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="f2601-106">Dispozitivul trebuie să aibă instalată aplicația portal firmă.</span><span class="sxs-lookup"><span data-stu-id="f2601-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="f2601-107">Dispozitivul trebuie să permită aplicației portal a firmei să trimită notificări Push.</span><span class="sxs-lookup"><span data-stu-id="f2601-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="f2601-108">Atunci când aplicația este instalată sau actualizată, aceasta va solicita utilizatorului să autorizeze notificările.</span><span class="sxs-lookup"><span data-stu-id="f2601-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="f2601-109">Dispozitivele Android trebuie să aibă instalat Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="f2601-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="f2601-110">Dispozitivul trebuie să fie înscris cu Intune.</span><span class="sxs-lookup"><span data-stu-id="f2601-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="f2601-111">Pentru mai multe informații, inclusiv cum să trimiteți un mesaj, consultați [documentația caracteristicii](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="f2601-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
