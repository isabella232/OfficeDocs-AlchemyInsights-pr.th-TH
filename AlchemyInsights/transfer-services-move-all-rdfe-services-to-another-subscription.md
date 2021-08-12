---
title: บริการถ่ายโอน - ย้ายบริการ RDFE ทั้งหมดไปยังการสมัครใช้งานอื่น
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
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940112"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>บริการถ่ายโอน - ย้ายบริการ RDFE ทั้งหมดไปยังการสมัครใช้งานอื่น

**ย้ายทรัพยากร**

แหล่งข้อมูล Azure สามารถย้ายไปยังการสมัครใช้งาน Azure หรือกลุ่มทรัพยากรอื่นภายใต้การสมัครใช้งานเดียวกันได้โดยใช้พอร์ทัล Azure, Azure PowerShell, Azure CLI หรือ REST API เพื่อย้ายทรัพยากร

ก่อนที่คุณจะสามารถย้ายแหล่งข้อมูล ให้ดู:

- [รายการตรวจสอบก่อนการย้ายทรัพยากร](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [บริการที่สามารถย้ายได้](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [วิธีการตรวจสอบการย้าย](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [ย้ายแนวทางสําหรับบริการ](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

เมื่อต้องการย้ายแหล่งข้อมูลที่มีอยู่ไปยังกลุ่มทรัพยากรหรือการสมัครใช้งานอื่น คุณสามารถใช้:

- [พอร์ทัล Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

บทช่วย [สอน: ย้ายแหล่งข้อมูล Azure ไปยังกลุ่มทรัพยากรหรือการสมัครใช้งานอื่น](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**แก้ไขข้อผิดพลาดด้วย Azure Resource Manager**

ดูบทความด้านล่างเพื่อเรียนรู้เกี่ยวกับข้อผิดพลาดทั่วไปในการปรับใช้ Azure บางส่วนและรับข้อมูลเพื่อแก้ไขปัญหา ถ้าคุณไม่พบรหัสข้อผิดพลาดของข้อผิดพลาดในการปรับใช้ ให้ดู[ค้นหารหัสข้อผิดพลาด](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [แก้ไขข้อผิดพลาดในการปรับใช้](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [แก้ไขปัญหาการย้ายแหล่งข้อมูล Azure ไปยังกลุ่มทรัพยากรหรือการสมัครใช้งานใหม่](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

โปรดทราบว่าหากคุณต้องการอัปเกรดการสมัครใช้งาน Azure ของคุณ เช่น สลับจากแบบฟรีเป็น pay-as-you-go คุณจะต้องแปลงการสมัครใช้งานของคุณ

- เมื่อต้องการอัปเกรดรุ่นทดลองใช้ฟรี ให้ดู[อัปเกรดการสมัครใช้งานเวอร์ชันทดลองใช้ฟรีหรือ Microsoft Imagine Azure เป็น Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- เมื่อต้องการเปลี่ยนบัญชีแบบจ่ายตามที่คุณใช้งาน ให้ดู [เปลี่ยนการสมัครใช้งาน Azure Pay-As-You-Go เป็นข้อเสนอ](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)อื่น

**เมื่อต้องการเพิ่มหรือเชื่อมโยงการสมัครใช้งาน Azure กับผู้Azure Active Directoryของคุณ:**

1. ลงชื่อเข้าใช้ และเลือกการสมัครใช้งานที่คุณต้องการใช้จากหน้า[การสมัครใช้งานในพอร์ทัล Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. เลือก **เปลี่ยน** ไดเรกทอรี
3. ตรวจสอบคําเตือนที่ปรากฏขึ้น **แล้วเลือก** เปลี่ยน
4. ไดเรกทอรีจะถูกเปลี่ยนในการสมัครใช้งาน และคุณจะได้รับข้อความแสดงความสเร็จ
5. ใช้ *ตัว* สลับไดเรกทอรีเพื่อไปยังไดเรกทอรีใหม่ของคุณ อาจใช้เวลาถึง 10 นาทีเพื่อให้ทุกอย่างแสดงขึ้นอย่างถูกต้อง

**เอกสารที่แนะนา**

- [การโอนสิทธิ์ความเป็นเจ้าของของการสมัครใช้งาน Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [ย้ายทรัพยากรไปยังกลุ่มทรัพยากรหรือการสมัครใช้งานใหม่](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [จัดการทรัพยากรโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
