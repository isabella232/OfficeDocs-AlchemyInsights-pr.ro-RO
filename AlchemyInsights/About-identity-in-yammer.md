---
title: Despre identitatea în Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664182"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="4dfaf-102">Despre identitatea în Yammer</span><span class="sxs-lookup"><span data-stu-id="4dfaf-102">About identity in Yammer</span></span>

<span data-ttu-id="4dfaf-103">Se recomandă ca toate rețelele să facă următorii pași pentru a evita problemele legate de identitate:</span><span class="sxs-lookup"><span data-stu-id="4dfaf-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="4dfaf-104">Impuneți identitatea Office 365 după asigurarea accesului conturilor Microsoft 365 pentru utilizatorii din Azure AD pentru a vă asigura că toți utilizatorii se conectează utilizând contul principal Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="4dfaf-105">Pentru mai multe informații, consultați [aplicarea identității Office 365 pentru utilizatorii Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="4dfaf-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="4dfaf-106">Sintetizarea mai multor rețele Yammer.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="4dfaf-107">Configurațiile Yammer moștenite permit conectarea mai multor rețele Yammer la o entitate găzduită.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="4dfaf-108">Pentru mai multe informații, consultați [migrarea rețelei-sintetizarea mai multor rețele Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="4dfaf-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="4dfaf-109">Opțional, aplicați licențierea pentru Yammer pentru a bloca utilizatorii din Yammer dacă nu au o licență.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="4dfaf-110">Pentru mai multe informații, consultați [gestionarea licențelor de utilizator Yammer în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4dfaf-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="4dfaf-111">În cele din urmă, auditați lista de utilizatori pentru rețelele Yammer mai vechi și suspendați utilizatorii moșteniti.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="4dfaf-112">Se recomandă să suspendați (să dezactivați) utilizatorii în loc să le ștergeți, deoarece ștergerea este ireversibilă.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="4dfaf-113">Pentru mai multe informații, consultați [auditarea utilizatorilor Yammer în rețelele conectate la Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) și [eliminarea utilizatorilor](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="4dfaf-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="4dfaf-114">Prin configurarea Yammer utilizând acești pași, veți fi, de asemenea, gata să configurați rețeaua Yammer pentru modul nativ pentru Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4dfaf-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="4dfaf-115">Pentru mai multe informații, consultați [configurarea rețelei Yammer pentru modul nativ pentru Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="4dfaf-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>