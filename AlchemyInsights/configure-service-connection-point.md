---
title: กําหนดค่าจุดเชื่อมต่อบริการ (SCP)
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
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037291"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="af377-102">กําหนดค่าจุดเชื่อมต่อบริการ (SCP)</span><span class="sxs-lookup"><span data-stu-id="af377-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="af377-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="af377-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="af377-104">**เหตุผล**: ไม่สามารถอ่านวัตถุ SCP และรับข้อมูลผู้เช่า Azure AD</span><span class="sxs-lookup"><span data-stu-id="af377-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="af377-105">**การแก้ปัญหา**: อ้างอิงไปยังส่วน [กําหนดค่าจุดเชื่อมต่อบริการ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="af377-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="af377-106">**แผนปฏิบัติการ**</span><span class="sxs-lookup"><span data-stu-id="af377-106">**Action plan**</span></span>

- <span data-ttu-id="af377-107">ตรวจสอบว่าอุปกรณ์ได้รับ GPO หรือไม่เกี่ยวกับการตรวจสอบความถูกต้องที่ควบคุม</span><span class="sxs-lookup"><span data-stu-id="af377-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="af377-108">ตรวจสอบให้แน่ใจว่า GPO ได้สร้างรีจิสทรีคีย์แล้ว</span><span class="sxs-lookup"><span data-stu-id="af377-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="af377-109">ตรวจสอบให้แน่ใจว่าคุณมี 2 คีย์ที่สร้างขึ้นด้วย ID ไดเรกทอรีและโดเมน onmicrosoft ของคุณ</span><span class="sxs-lookup"><span data-stu-id="af377-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="af377-110">**การกําหนดค่าการตั้งค่ารีจิสทรีที่ฝั่งไคลเอ็นต์ของ SCP**</span><span class="sxs-lookup"><span data-stu-id="af377-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="af377-111">ใช้ตัวอย่างต่อไปนี้เพื่อสร้าง Group Policy Object (GPO) เพื่อปรับใช้การตั้งค่ารีจิสทรีที่กําหนดค่ารายการ SCP ในรีจิสทรีของอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="af377-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="af377-112">เปิดคอนโซลการจัดการนโยบายกลุ่มและสร้าง GPO ใหม่ในโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="af377-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="af377-113">ใส่ชื่อ GPO ที่สร้างขึ้นใหม่ของคุณ (ตัวอย่างเช่น ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="af377-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="af377-114">แก้ไข GPO และค้นหาเส้นทางต่อไปนี้: การกําหนดค่า **>กําหนด>กําหนดลักษณะ> Windows >รีจิสทรี**</span><span class="sxs-lookup"><span data-stu-id="af377-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="af377-115">คลิกขวาที่รีจิสทรี **แล้วเลือกรายการ\*\*\*\*รีจิสทรี>ใหม่**</span><span class="sxs-lookup"><span data-stu-id="af377-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="af377-116">บนแท็บ **ทั่วไป** ให้กําหนดค่าต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="af377-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="af377-117">**การปฏิบัติการ**: อัปเดต</span><span class="sxs-lookup"><span data-stu-id="af377-117">**Action**: Update</span></span>
    
- <span data-ttu-id="af377-118">**ไฮฟ์**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="af377-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="af377-119">**เส้นทางคีย์**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="af377-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="af377-120">**ชื่อค่า**: TenantId</span><span class="sxs-lookup"><span data-stu-id="af377-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="af377-121">**ชนิดของค่า**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="af377-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="af377-122">**ข้อมูลค่า**: GUID หรือ ID ไดเรกทอรีของอินสแตนซ์ Azure AD ของคุณ (ค่านี้สามารถพบได้ในพอร์ทัล **Azure > Azure Active Directory > Properties > Directory ID)**</span><span class="sxs-lookup"><span data-stu-id="af377-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="af377-123">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="af377-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="af377-124">คลิกขวาที่รีจิสทรี **แล้วเลือกรายการ\*\*\*\*รีจิสทรี>ใหม่**</span><span class="sxs-lookup"><span data-stu-id="af377-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="af377-125">บนแท็บ **ทั่วไป** ให้กําหนดค่าต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="af377-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="af377-126">**การปฏิบัติการ**: อัปเดต</span><span class="sxs-lookup"><span data-stu-id="af377-126">**Action**: Update</span></span>
    
- <span data-ttu-id="af377-127">**ไฮฟ์**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="af377-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="af377-128">**เส้นทางคีย์**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="af377-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="af377-129">**ชื่อค่า**: TenantName</span><span class="sxs-lookup"><span data-stu-id="af377-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="af377-130">**ชนิดค่า**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="af377-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="af377-131">**ข้อมูลค่า**: ชื่อโดเมนที่ตรวจสอบแล้วของคุณถ้าคุณใช้สภาพแวดล้อมภายนอก เช่น AD FS</span><span class="sxs-lookup"><span data-stu-id="af377-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="af377-132">ชื่อโดเมนที่ตรวจสอบแล้วหรือชื่อโดเมน onmicrosoft.com ของคุณ (ตัวอย่างเช่น contoso.onmicrosoft).com ถ้าคุณใช้งานสภาพแวดล้อมที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="af377-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="af377-133">คลิก **OK**</span><span class="sxs-lookup"><span data-stu-id="af377-133">Click **OK**.</span></span>

7. <span data-ttu-id="af377-134">ปิดตัวแก้ไขของ GPO ที่สร้างขึ้นใหม่</span><span class="sxs-lookup"><span data-stu-id="af377-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="af377-135">ลิงก์ GPO ที่สร้างขึ้นใหม่ไปยัง OU ที่ต้องการซึ่งมีคอมพิวเตอร์ที่เข้าร่วมโดเมนที่เป็นของประชากรที่เริ่มใช้ที่ควบคุมของคุณ</span><span class="sxs-lookup"><span data-stu-id="af377-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="af377-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | เอกสาร Microsoft และ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)การแก้ไขปัญหา[อุปกรณ์ที่เข้าร่วมของ Azure Active Directory แบบ| เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)</span><span class="sxs-lookup"><span data-stu-id="af377-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









