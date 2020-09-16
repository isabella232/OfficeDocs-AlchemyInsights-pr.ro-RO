---
title: Probleme de performanță-SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771256"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="9833c-102">SharePoint sau OneDrive este lent, inaccesibil sau indisponibil pentru mai mulți utilizatori</span><span class="sxs-lookup"><span data-stu-id="9833c-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="9833c-103">Dacă un site OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut acces anterior, este posibil să existe o problemă de serviciu temporară.</span><span class="sxs-lookup"><span data-stu-id="9833c-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="9833c-104">[Verificați tabloul de bord pentru starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="9833c-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="9833c-105">**Adăugarea și licența utilizatorului**</span><span class="sxs-lookup"><span data-stu-id="9833c-105">**Add and license the user**</span></span>

<span data-ttu-id="9833c-106">Asigurați-vă că [atribuiți licențe utilizatorilor din Microsoft 365 pentru Business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="9833c-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="9833c-107">**Atribuirea permisiunilor**</span><span class="sxs-lookup"><span data-stu-id="9833c-107">**Assign Permissions**</span></span>

<span data-ttu-id="9833c-108">Dacă utilizatorului i s-a atribuit o licență SharePoint și încă primește un mesaj de acces refuzat, asigurați-vă că au atribuit [nivelul de permisiune corespunzător](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="9833c-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="9833c-109">**Luați în considerare utilizarea caracteristicii de solicitare de acces**</span><span class="sxs-lookup"><span data-stu-id="9833c-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="9833c-110">[Caracteristica de solicitare de acces](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite persoanelor să solicite acces la conținut pe care nu le pot vedea momentan.</span><span class="sxs-lookup"><span data-stu-id="9833c-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="9833c-111">**Permiteți ca scriptul particularizat să provoace probleme de acces refuzat**</span><span class="sxs-lookup"><span data-stu-id="9833c-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="9833c-112">Există anumite scenarii în care *opțiunea se permite script particularizat* să prezinte un acces refuzat.</span><span class="sxs-lookup"><span data-stu-id="9833c-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="9833c-113">Pentru o listă de caracteristici afectate, considerații de securitate și capacitatea de a dezactiva caracteristica.</span><span class="sxs-lookup"><span data-stu-id="9833c-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="9833c-114">Vă rugăm să vizitați [Permiteți sau să împiedicați scriptul particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="9833c-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

