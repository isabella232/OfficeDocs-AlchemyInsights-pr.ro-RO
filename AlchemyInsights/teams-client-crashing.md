---
title: Clientul Teams are căderi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030676"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="492c4-102">Clientul Teams are căderi?</span><span class="sxs-lookup"><span data-stu-id="492c4-102">Teams client crashing?</span></span>

<span data-ttu-id="492c4-103">Dacă clientul dvs. Teams are căderi, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="492c4-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="492c4-104">Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="492c4-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="492c4-105">Asigurați-vă că toate [URL-urile și intervalele de adrese Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sunt accesibile.</span><span class="sxs-lookup"><span data-stu-id="492c4-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="492c4-106">Conectați-vă cu contul dvs. de administrator și verificați [Tabloul de bord cu starea serviciilor](https://docs.microsoft.com/office365/enterprise/view-service-health) pentru a verifica dacă există vreo întrerupere sau degradare a serviciului.</span><span class="sxs-lookup"><span data-stu-id="492c4-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="492c4-107">Ca ultim pas, puteți încerca să goliți memoria cache a clientului Teams:</span><span class="sxs-lookup"><span data-stu-id="492c4-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="492c4-108">Ieșiți complet din clientul desktop Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="492c4-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="492c4-109">Puteți să faceți dreapta pe **Teams** din bara de pictograme, apoi să faceți clic pe **Ieșire** sau să rulați Manager de activități și să anihilați complet procesul.</span><span class="sxs-lookup"><span data-stu-id="492c4-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="492c4-110">Mergeți la Explorer și tastați %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="492c4-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="492c4-111">Când vă aflați în director, veți vedea câteva dintre următoarele foldere:</span><span class="sxs-lookup"><span data-stu-id="492c4-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="492c4-112">Din **Application Cache**, accesați Cache și ștergeți orice fișier din locația de cache: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="492c4-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="492c4-113">Din **Blob_storage**, ștergeți toate fișierele: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="492c4-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="492c4-114">Din **Cache**, ștergeți toate fișierele: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="492c4-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="492c4-115">Din **databases**, ștergeți toate fișierele: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="492c4-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="492c4-116">Din **GPUCache**, ștergeți toate fișierele: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="492c4-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="492c4-117">Din **IndexedDB**, ștergeți fișierul .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="492c4-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="492c4-118">Din **Local Storage**, ștergeți toate fișierele: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="492c4-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="492c4-119">În final, din **tmp**, ștergeți orice fișier: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="492c4-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="492c4-120">Reporniți clientul Teams.</span><span class="sxs-lookup"><span data-stu-id="492c4-120">Restart your Teams client.</span></span>
