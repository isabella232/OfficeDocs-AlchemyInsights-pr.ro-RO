---
title: Portați extensii Google Chrome la Microsoft Edge (crom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678984"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="af371-102">Portați extensii Google Chrome la Microsoft Edge (crom)</span><span class="sxs-lookup"><span data-stu-id="af371-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="af371-103">Este ușor să [portați extensii Google Chrome la Microsoft Edge (crom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="af371-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="af371-104">În majoritatea cazurilor, sunt necesare doar modificări minime pentru a executa aceste extensii în Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="af371-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="af371-105">API-urile de extensie și tastele manifest acceptate de Google Chrome sunt compatibile cu codul cu Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="af371-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="af371-106">Cu toate acestea, Microsoft Edge nu acceptă extensia APIs Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken și Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="af371-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>