---
title: Set de reproduceri
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714255"
---
# <a name="replica-set"></a><span data-ttu-id="34f5d-102">Set de reproduceri</span><span class="sxs-lookup"><span data-stu-id="34f5d-102">Replica set</span></span>

<span data-ttu-id="34f5d-103">AADDS este, de asemenea, denumit domeniul gestionat.</span><span class="sxs-lookup"><span data-stu-id="34f5d-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="34f5d-104">De fapt, sunt două controlere de domeniu care rulează și sunt întreținute de backend.</span><span class="sxs-lookup"><span data-stu-id="34f5d-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="34f5d-105">Cele două DCs includ un DC principal și unul de replicare DC.</span><span class="sxs-lookup"><span data-stu-id="34f5d-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="34f5d-106">Backupurile din AADDS (domeniul gestionat) sunt un proces automatizat gestionat de platforma Azure.</span><span class="sxs-lookup"><span data-stu-id="34f5d-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="34f5d-107">În cazul unei probleme cu domeniul gestionat, asistența Azure vă poate ajuta în restaurarea din backup.</span><span class="sxs-lookup"><span data-stu-id="34f5d-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="34f5d-108">Creați fiecare set de reproduceri într-o rețea virtuală.</span><span class="sxs-lookup"><span data-stu-id="34f5d-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="34f5d-109">Fiecare rețea virtuală trebuie să fie coordonată fiecărei rețele virtuale care găzduiește un set de reproduceri al domeniului gestionat.</span><span class="sxs-lookup"><span data-stu-id="34f5d-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="34f5d-110">Această configurație creează o topologie de rețea Mesh care acceptă reproducerea directorului.</span><span class="sxs-lookup"><span data-stu-id="34f5d-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="34f5d-111">O rețea virtuală poate accepta mai multe seturi de replicare, cu condiția ca fiecare set de reproduceri să se află într-o subrețea virtuală diferită.</span><span class="sxs-lookup"><span data-stu-id="34f5d-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="34f5d-112">Pentru mai multe detalii despre setul de reproduceri, consultați [seturi de reproduceri concepte](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="34f5d-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
