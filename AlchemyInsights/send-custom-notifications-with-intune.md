---
title: Trimiteți notificări personalizate cu Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992324"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="d1f99-102">să trimiteți notificări personalizate utilizatorilor de dispozitive iOS și Android gestionate</span><span class="sxs-lookup"><span data-stu-id="d1f99-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="d1f99-103">Notificările particularizate pentru Intune sunt procesate de aplicația portal de companie pe dispozitivul unui utilizator.</span><span class="sxs-lookup"><span data-stu-id="d1f99-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="d1f99-104">Aplicația apoi creează notificarea Push pe acel dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="d1f99-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="d1f99-105">Următoarele sunt premise pentru dispozitiv pentru a accepta primirea notificărilor particularizate și pentru ca aplicația să creeze apoi notificarea Push:</span><span class="sxs-lookup"><span data-stu-id="d1f99-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="d1f99-106">Dispozitivul trebuie să aibă instalată aplicația portal de companie.</span><span class="sxs-lookup"><span data-stu-id="d1f99-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="d1f99-107">Dispozitivul trebuie să permită aplicației portal companie să trimită notificări Push.</span><span class="sxs-lookup"><span data-stu-id="d1f99-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="d1f99-108">Când aplicația este instalată sau actualizată, va solicita utilizatorului să permită notificări.</span><span class="sxs-lookup"><span data-stu-id="d1f99-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="d1f99-109">Dispozitivele Android trebuie să aibă instalat serviciile Google Play.</span><span class="sxs-lookup"><span data-stu-id="d1f99-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="d1f99-110">Dispozitivul trebuie să fie înscris cu Intune.</span><span class="sxs-lookup"><span data-stu-id="d1f99-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="d1f99-111">Pentru mai multe informații, inclusiv să trimiteți un mesaj, consultați [documentația caracteristică](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="d1f99-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
