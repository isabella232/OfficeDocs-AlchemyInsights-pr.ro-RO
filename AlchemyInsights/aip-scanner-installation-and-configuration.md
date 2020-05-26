---
title: 'Scaner AIP: instalare și configurare'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358105"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="5b675-102">Scaner AIP: instalare și configurare</span><span class="sxs-lookup"><span data-stu-id="5b675-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="5b675-103">**Pentru a instala scanerul AIP, urmați instrucțiunile recomandate:**</span><span class="sxs-lookup"><span data-stu-id="5b675-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="5b675-104">Dacă faceți upgrade și nu efectuați o instalare curată, asigurați-vă că ați urmat instrucțiunile pentru [upgrade-ul scanerului Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) și pentru clientul unificat de etichetare, consultați [upgrade-ul scanerului Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="5b675-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="5b675-105">Verificați dacă respectați toate [cerințele privind paravanele de protecție și setările de infrastructură de rețea](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="5b675-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="5b675-106">Asigurați-vă că [politicile sunt setate](https://docs.microsoft.com/azure/information-protection/configure-policy) la etichetare automată sau că aveți o etichetă implicită în politică.</span><span class="sxs-lookup"><span data-stu-id="5b675-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="5b675-107">Asigurați-vă că tipul de fișier relevant este configurat pentru etichetă/protecție așa este descris în [tipuri de fișiere acceptate de clientul Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="5b675-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="5b675-108">În plus, dacă doriți să modificați comportamentul implicit, urmați aceste instrucțiuni: [Modificarea nivelului implicit de protecție a fișierelor](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="5b675-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="5b675-109">Verificați că contul de utilizator configurat pentru a executa serviciul de scaner are permisiuni pentru a accesa toate depozitele configurate.</span><span class="sxs-lookup"><span data-stu-id="5b675-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="5b675-110">Dacă întâmpinați în continuare probleme, exportați jurnalele scanerului și adăugați-le la biletul de asistență.</span><span class="sxs-lookup"><span data-stu-id="5b675-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="5b675-111">**Export azure informații protecție scaner jurnalele**</span><span class="sxs-lookup"><span data-stu-id="5b675-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="5b675-112">Navigați la %localappdata%\Microsoft\MSIP sub contextul utilizatorului care execută serviciul de scanare.</span><span class="sxs-lookup"><span data-stu-id="5b675-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="5b675-113">Zip tot conținutul sub folderul MSIP.</span><span class="sxs-lookup"><span data-stu-id="5b675-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="5b675-114">Salvați jurnalele la alegerea locației și atașați-le la solicitarea de serviciu.</span><span class="sxs-lookup"><span data-stu-id="5b675-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="5b675-115">Puteți utiliza, de asemenea, [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="5b675-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="5b675-116">**Pentru informații suplimentare, consultați:**</span><span class="sxs-lookup"><span data-stu-id="5b675-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="5b675-117">Implementarea scanerului Azure Information Protection pentru a clasifica și proteja automat fișierele</span><span class="sxs-lookup"><span data-stu-id="5b675-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="5b675-118">Specificați și utilizați parametrul Simbol pentru Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="5b675-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="5b675-119">Executarea unui ciclu de descoperire și vizualizarea rapoartelor pentru scaner</span><span class="sxs-lookup"><span data-stu-id="5b675-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="5b675-120">Examinați documentația Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5b675-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="5b675-121">Cerințe pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5b675-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="5b675-122">Descărcați clientul Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5b675-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
