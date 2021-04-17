---
title: อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณกับผู้ให้บริการโฮสต์ปัจจุบันของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827558"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณกับผู้ให้บริการโฮสต์ปัจจุบันของคุณ

1. ในศูนย์การจัดการ Microsoft 365 ให้ไปที่หน้าตั้งค่าโดเมน และในรายการโดเมน  >  [](https://admin.microsoft.com/Adminportal#/Domains)ให้เลือกโดเมนที่คุณใช้กับเว็บไซต์ของคุณ

2. เลือก **+ ระเบียนแบบปรับแต่งเอง** ใหม่ แล้วใส่ข้อมูลต่อไปนี้:

  - For **DNS type** enter: A **(Address)**

  - For **Host name or Alias**, type the following: **@**

  - For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).

    ซึ่ง  *ต้องเป็นที่อยู่*  IP แบบคงที่ของเว็บไซต์ ไม่ใช่  *ที่อยู่*  IP แบบไดนามิก ตรวจสอบกับไซต์ที่เว็บไซต์ของคุณถูกโฮสต์เพื่อให้แน่ใจว่าคุณสามารถรับที่อยู่ IP แบบคงที่ของเว็บไซต์สาธารณะของคุณ

3. เลือกบันทึก

นอกจากนี้ คุณสามารถสร้างระเบียน CNAME เพื่อช่วยให้ลูกค้าค้นหาเว็บไซต์ของคุณได้
  
1. เลือก **+ ระเบียนแบบปรับแต่งเอง** ใหม่ แล้วใส่ข้อมูลต่อไปนี้:

  - For **DNS type** enter: **CNAME (Alias)**

  - For **Host name or Alias**, type the following: **www**

  - For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).

2. เลือกบันทึก
