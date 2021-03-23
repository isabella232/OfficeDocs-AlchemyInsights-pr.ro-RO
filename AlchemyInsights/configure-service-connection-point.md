---
title: Configurarea punctului de conexiune la serviciu (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037286"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="0a98f-102">Configurarea punctului de conexiune la serviciu (SCP)</span><span class="sxs-lookup"><span data-stu-id="0a98f-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="0a98f-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="0a98f-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="0a98f-104">**Motiv**: imposibilitatea de a citi obiectul SCP și de a obține informații despre entitatea găzduită Azure AD</span><span class="sxs-lookup"><span data-stu-id="0a98f-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="0a98f-105">**Rezolvare**: consultați secțiunea [Configurarea unui punct de conexiune la serviciu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="0a98f-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="0a98f-106">**Plan de acțiune**</span><span class="sxs-lookup"><span data-stu-id="0a98f-106">**Action plan**</span></span>

- <span data-ttu-id="0a98f-107">Verificați dacă dispozitivul a primit obiectul GPO pentru validarea controlată.</span><span class="sxs-lookup"><span data-stu-id="0a98f-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="0a98f-108">Asigurați-vă că obiectul GPO a creat cheile de registry.</span><span class="sxs-lookup"><span data-stu-id="0a98f-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="0a98f-109">Asigurați-vă că aveți 2 taste create cu ID-ul de director și cu domeniul onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="0a98f-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="0a98f-110">**Configurarea setării de registry pe partea client pentru SCP**</span><span class="sxs-lookup"><span data-stu-id="0a98f-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="0a98f-111">Utilizați următorul exemplu pentru a crea un obiect politică de grup (GPO) pentru a implementa o setare de registry ce configurează o intrare SCP în registry-ul dispozitivelor dvs.</span><span class="sxs-lookup"><span data-stu-id="0a98f-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="0a98f-112">Deschideți o consolă de gestionare a politicilor de grup și creați un nou GPO în domeniul dvs.</span><span class="sxs-lookup"><span data-stu-id="0a98f-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="0a98f-113">Furnizați un nume GPO nou creat (de exemplu, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="0a98f-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="0a98f-114">Editați obiectul GPO și găsiți următoarea cale: **Configurarea computerului > preferințe > setările Windows > registry**.</span><span class="sxs-lookup"><span data-stu-id="0a98f-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="0a98f-115">Faceți clic dreapta pe **registry** și selectați **nou > element de registry**.</span><span class="sxs-lookup"><span data-stu-id="0a98f-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="0a98f-116">Pe fila **General** , configurați următoarele:</span><span class="sxs-lookup"><span data-stu-id="0a98f-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="0a98f-117">**Acțiune**: actualizare</span><span class="sxs-lookup"><span data-stu-id="0a98f-117">**Action**: Update</span></span>
    
- <span data-ttu-id="0a98f-118">**Stup**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="0a98f-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="0a98f-119">**Cale cheie**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="0a98f-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="0a98f-120">**Nume valoare**: TenantId</span><span class="sxs-lookup"><span data-stu-id="0a98f-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="0a98f-121">**Tip de valoare**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="0a98f-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="0a98f-122">**Date valoare**: ID-ul GUID sau director al instanței de publicitate Azure (această valoare poate fi găsită în **Azure portal > azure Active Directory > proprietăți > ID Director**)</span><span class="sxs-lookup"><span data-stu-id="0a98f-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="0a98f-123">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="0a98f-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="0a98f-124">Faceți clic dreapta pe **registry** și selectați **nou > element de registry**.</span><span class="sxs-lookup"><span data-stu-id="0a98f-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="0a98f-125">Pe fila **General** , configurați următoarele:</span><span class="sxs-lookup"><span data-stu-id="0a98f-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="0a98f-126">**Acțiune**: actualizare</span><span class="sxs-lookup"><span data-stu-id="0a98f-126">**Action**: Update</span></span>
    
- <span data-ttu-id="0a98f-127">**Stup**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="0a98f-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="0a98f-128">**Cale cheie**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="0a98f-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="0a98f-129">**Nume valoare**: TenantName</span><span class="sxs-lookup"><span data-stu-id="0a98f-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="0a98f-130">**Tip de valoare**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="0a98f-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="0a98f-131">**Date valoare**: numele de domeniu verificat dacă utilizați mediul federativ, cum ar fi AD FS.</span><span class="sxs-lookup"><span data-stu-id="0a98f-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="0a98f-132">Numele de domeniu verificat sau numele de domeniu onmicrosoft.com (de exemplu, contoso. onmicrosoft). com Dacă utilizați mediu gestionat</span><span class="sxs-lookup"><span data-stu-id="0a98f-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="0a98f-133">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="0a98f-133">Click **OK**.</span></span>

7. <span data-ttu-id="0a98f-134">Închideți editorul pentru GPO-ul nou creat.</span><span class="sxs-lookup"><span data-stu-id="0a98f-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="0a98f-135">Legați GPO-ul nou creat la OU-ul dorit care conține computere asociate domeniului care aparțin populației de implementare controlată.</span><span class="sxs-lookup"><span data-stu-id="0a98f-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="0a98f-136">Pentru mai multe informații, consultați [validarea controlată a asocierii hibride AZURE AD-AZURE AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) și  [depanarea dispozitivelor hibride Azure Active Directory asociate | Documente Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="0a98f-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









