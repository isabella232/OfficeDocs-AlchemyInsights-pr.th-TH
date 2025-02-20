---
title: การกําหนดค่าจุดเชื่อมต่อบริการ (SCP)
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
ms.openlocfilehash: 5ccb55996ccef4b55c8d80de6e35f4ba27e3dfa18dfcaeaf6f6ad1c54b6bb376
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965984"
---
# <a name="configure-service-connection-point-scp"></a>การกําหนดค่าจุดเชื่อมต่อบริการ (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **เหตุผล**: ไม่สามารถอ่านวัตถุ SCP และรับข้อมูลผู้เช่า Azure AD
- **การแก้ปัญหา**: อ้างอิงส่วน [กําหนดค่าจุดเชื่อมต่อบริการ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**แผนปฏิบัติการ**

- ตรวจสอบว่าอุปกรณ์ได้รับ GPO หรือไม่ เพื่อการตรวจสอบความถูกต้องที่ควบคุม
- ตรวจสอบให้แน่ใจว่า GPO ได้สร้างรีจิสทรีคีย์แล้ว
- ตรวจสอบให้แน่ใจว่าคุณมี 2 คีย์ที่สร้างขึ้นด้วย ID ไดเรกทอรีและโดเมน onmicrosoft ของคุณ

**การกําหนดค่าการตั้งค่ารีจิสทรีฝั่งไคลเอ็นต์ของ SCP**

ใช้ตัวอย่างต่อไปนี้เพื่อสร้าง Group Policy Object (GPO) เพื่อปรับใช้การตั้งค่ารีจิสทรีที่กําหนดค่ารายการ SCP ในรีจิสทรีของอุปกรณ์ของคุณ

1. เปิดคอนโซลการจัดการนโยบายกลุ่มและสร้าง GPO ใหม่ในโดเมนของคุณ
     - ใส่ชื่อ GPO ที่สร้างขึ้นใหม่ของคุณ (ตัวอย่างเช่น ClientSideSCP)

2. แก้ไข GPO และค้นหาเส้นทางต่อไปนี้:**การกําหนดค่า>กําหนด> Windows การตั้งค่า >กําหนด> Windows การตั้งค่า >รีจิสทรี**

3. คลิกขวาที่รีจิสทรี **แล้วเลือก รายการ****>รีจิสทรีใหม่**

4. บนแท็บ **ทั่วไป** ให้กําหนดค่าต่อไปนี้:
  
- **การแอคชัน**: อัปเดต
    
- **ไฮฟ์**: HKEY_LOCAL_MACHINE
    
- **เส้นทางคีย์**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **ชื่อค่า**: TenantId
    
- **ชนิดค่า**: REG_SZ
    
- **ข้อมูลค่า**: GUID หรือ ID ไดเรกทอรีของอินสแตนซ์ Azure AD ของคุณ (ค่านี้สามารถพบได้ในพอร์ทัล Azure > Azure Active Directory > **Properties > Directory ID**)
 
- คลิก **OK**
 
5. คลิกขวาที่รีจิสทรี **แล้วเลือก รายการ****>รีจิสทรีใหม่**

6. บนแท็บ **ทั่วไป** ให้กําหนดค่าต่อไปนี้:
  
- **การแอคชัน**: อัปเดต
    
- **ไฮฟ์**: HKEY_LOCAL_MACHINE
    
- **เส้นทางคีย์**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **ชื่อค่า**: TenantName
    
- **ชนิดค่า**: REG_SZ
    
- **ข้อมูลค่า**: ชื่อโดเมนที่ตรวจสอบแล้วของคุณถ้าคุณใช้สภาพแวดล้อมภายนอก เช่น AD FS ชื่อโดเมนที่ตรวจสอบแล้วหรือชื่อโดเมน onmicrosoft.com ของคุณ (ตัวอย่างเช่น contoso.onmicrosoft).com ถ้าคุณจะใช้สภาพแวดล้อมที่มีการจัดการ

- คลิก **OK**

7. ปิดตัวแก้ไขของ GPO ที่สร้างขึ้นใหม่

8. ลิงก์ GPO ที่สร้างขึ้นใหม่ไปยัง OU ที่ต้องการซึ่งมีคอมพิวเตอร์ที่เข้าร่วมโดเมนที่เป็นของประชากรที่เริ่มใช้ที่ควบคุมของคุณ

For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | เอกสาร Microsoft และ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)การแก้ไขปัญหา[รุ่นAzure Active Directoryอุปกรณ์ที่เข้าร่วม| เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)









