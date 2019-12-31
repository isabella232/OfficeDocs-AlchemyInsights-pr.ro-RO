---
title: Administrarea concomitentă
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910406"
---
# <a name="co-management"></a><span data-ttu-id="0d19f-102">Administrarea concomitentă</span><span class="sxs-lookup"><span data-stu-id="0d19f-102">Co-management</span></span>

<span data-ttu-id="0d19f-103">**Cerințe preliminare pentru migrarea de la config Manager hibrid la Intune**</span><span class="sxs-lookup"><span data-stu-id="0d19f-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="0d19f-104">Examinați [acest articol](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span><span class="sxs-lookup"><span data-stu-id="0d19f-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="0d19f-105">[Adăugați o licență Intune utilizatorilor](https://docs.microsoft.com/intune/licenses-assign).</span><span class="sxs-lookup"><span data-stu-id="0d19f-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="0d19f-106">Utilizați [browserul Edge](https://www.microsoft.com/windows/microsoft-edge) la configurarea co-management.</span><span class="sxs-lookup"><span data-stu-id="0d19f-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="0d19f-107">**se instalează clientul config Manager pe dispozitive gestionate Intune**</span><span class="sxs-lookup"><span data-stu-id="0d19f-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="0d19f-108">Vedeți [dispozitivele Windows gestionate de la Intune MDM](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span><span class="sxs-lookup"><span data-stu-id="0d19f-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="0d19f-109">**Ce se va face dacă vreau doar să schimb autoritatea MDM?**</span><span class="sxs-lookup"><span data-stu-id="0d19f-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="0d19f-110">Autoritatea MDM poate fi schimbată fără a deschide un caz de suport.</span><span class="sxs-lookup"><span data-stu-id="0d19f-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="0d19f-111">Vă rugăm să consultați documentația următoare pentru a ajuta la schimbarea autorității MDM:</span><span class="sxs-lookup"><span data-stu-id="0d19f-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="0d19f-112">Scimbare MDM autoritate de la config conducător la spre Intune standalone</span><span class="sxs-lookup"><span data-stu-id="0d19f-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="0d19f-113">Scimbare MDM autoritate de la Intune standalone la spre config conducător</span><span class="sxs-lookup"><span data-stu-id="0d19f-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)