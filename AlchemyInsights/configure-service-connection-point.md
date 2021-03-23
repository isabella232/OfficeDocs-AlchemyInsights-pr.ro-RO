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
# <a name="configure-service-connection-point-scp"></a>Configurarea punctului de conexiune la serviciu (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Motiv**: imposibilitatea de a citi obiectul SCP și de a obține informații despre entitatea găzduită Azure AD
- **Rezolvare**: consultați secțiunea [Configurarea unui punct de conexiune la serviciu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Plan de acțiune**

- Verificați dacă dispozitivul a primit obiectul GPO pentru validarea controlată.
- Asigurați-vă că obiectul GPO a creat cheile de registry.
- Asigurați-vă că aveți 2 taste create cu ID-ul de director și cu domeniul onmicrosoft.

**Configurarea setării de registry pe partea client pentru SCP**

Utilizați următorul exemplu pentru a crea un obiect politică de grup (GPO) pentru a implementa o setare de registry ce configurează o intrare SCP în registry-ul dispozitivelor dvs.

1. Deschideți o consolă de gestionare a politicilor de grup și creați un nou GPO în domeniul dvs.
     - Furnizați un nume GPO nou creat (de exemplu, ClientSideSCP)

2. Editați obiectul GPO și găsiți următoarea cale: **Configurarea computerului > preferințe > setările Windows > registry**.

3. Faceți clic dreapta pe **registry** și selectați **nou > element de registry**.

4. Pe fila **General** , configurați următoarele:
  
- **Acțiune**: actualizare
    
- **Stup**: HKEY_LOCAL_MACHINE
    
- **Cale cheie**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nume valoare**: TenantId
    
- **Tip de valoare**: REG_SZ
    
- **Date valoare**: ID-ul GUID sau director al instanței de publicitate Azure (această valoare poate fi găsită în **Azure portal > azure Active Directory > proprietăți > ID Director**)
 
- Faceți clic pe **OK**.
 
5. Faceți clic dreapta pe **registry** și selectați **nou > element de registry**.

6. Pe fila **General** , configurați următoarele:
  
- **Acțiune**: actualizare
    
- **Stup**: HKEY_LOCAL_MACHINE
    
- **Cale cheie**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nume valoare**: TenantName
    
- **Tip de valoare**: REG_SZ
    
- **Date valoare**: numele de domeniu verificat dacă utilizați mediul federativ, cum ar fi AD FS. Numele de domeniu verificat sau numele de domeniu onmicrosoft.com (de exemplu, contoso. onmicrosoft). com Dacă utilizați mediu gestionat

- Faceți clic pe **OK**.

7. Închideți editorul pentru GPO-ul nou creat.

8. Legați GPO-ul nou creat la OU-ul dorit care conține computere asociate domeniului care aparțin populației de implementare controlată.

Pentru mai multe informații, consultați [validarea controlată a asocierii hibride AZURE AD-AZURE AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) și  [depanarea dispozitivelor hibride Azure Active Directory asociate | Documente Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









