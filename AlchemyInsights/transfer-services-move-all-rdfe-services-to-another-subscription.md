---
title: บริการถ่ายโอน-ย้ายบริการ RDFE ทั้งหมดไปยังการสมัครใช้งานอื่น
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692179"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>บริการถ่ายโอน-ย้ายบริการ RDFE ทั้งหมดไปยังการสมัครใช้งานอื่น

**ย้ายทรัพยากร**

ทรัพยากร azure สามารถย้ายไปยังการสมัครใช้งาน Azure หรือกลุ่มทรัพยากรอื่นภายใต้การสมัครใช้งานเดียวกันได้โดยใช้ Azure portal, Azure PowerShell, Azure CLI หรือส่วนที่เหลือ API เพื่อย้ายทรัพยากร

ก่อนที่คุณจะสามารถย้ายแหล่งข้อมูลให้ดูที่:

- [รายการตรวจสอบก่อนที่จะย้ายทรัพยากร](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [บริการที่สามารถย้ายได้](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [วิธีตรวจสอบความถูกต้องของการย้าย](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [ย้ายคำแนะนำสำหรับบริการ](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

เมื่อต้องการย้ายแหล่งข้อมูลที่มีอยู่ไปยังกลุ่มทรัพยากรอื่นหรือการสมัครใช้งานคุณสามารถใช้:

- [พอร์ทัล Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

บทช่วยสอน:[ย้ายทรัพยากร Azure ไปยังกลุ่มทรัพยากรอื่นหรือการสมัคร](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)ใช้งาน

**การแก้ไขปัญหาข้อผิดพลาดด้วยตัวจัดการทรัพยากร Azure**

ดูบทความด้านล่างนี้เพื่อเรียนรู้เกี่ยวกับข้อผิดพลาดในการปรับใช้ Azure ทั่วไปและรับข้อมูลเพื่อแก้ไขปัญหาเหล่านั้น ถ้าคุณไม่พบรหัสข้อผิดพลาดสำหรับข้อผิดพลาดในการปรับใช้ของคุณให้ดูที่[ค้นหารหัสข้อผิดพลาด](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [การแก้ไขปัญหาข้อผิดพลาดในการปรับใช้](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [การแก้ไขปัญหาการย้ายทรัพยากร Azure ไปยังกลุ่มทรัพยากรใหม่หรือการสมัครใช้งาน](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

โปรดทราบว่าถ้าคุณต้องการอัปเกรดการสมัครใช้งาน Azure ของคุณเช่นการสลับจากค่าใช้จ่ายที่ไม่มีค่าใช้จ่ายในขณะเดินทางคุณจะต้องแปลงการสมัครใช้งานของคุณ

- เมื่อต้องการอัปเกรดเวอร์ชันทดลองใช้ฟรีให้ดูที่[อัปเกรดเวอร์ชันทดลองใช้ฟรีของคุณหรือ Microsoft ลองใช้การสมัครใช้งาน Azure เพื่อชำระเงินตามที่คุณไป](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- เมื่อต้องการเปลี่ยนบัญชีผู้ใช้แบบชำระเงินเป็นแบบของคุณให้ดูที่[เปลี่ยนการสมัครใช้งานแบบชำระเงินของ Azure ของคุณไปยังข้อเสนออื่น](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**เมื่อต้องการเพิ่มหรือเชื่อมโยงการสมัครใช้งาน Azure กับผู้เช่า Azure Active directory ของคุณให้ทำดังนี้**

1. ลงชื่อเข้าใช้และเลือกการสมัครใช้งานที่คุณต้องการใช้จากหน้าการสมัครใช้งาน[ใน Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. เลือก **เปลี่ยนไดเรกทอรี**
3. ตรวจทานคำเตือนที่ปรากฏขึ้นจากนั้นเลือก **เปลี่ยน**
4. ไดเรกทอรีจะถูกเปลี่ยนแปลงสำหรับการสมัครใช้งานและคุณจะได้รับข้อความแสดงความสำเร็จ
5. ใช้ตัวสลับ *ไดเรกทอรี* เพื่อไปที่ไดเรกทอรีใหม่ของคุณ อาจใช้เวลาถึง10นาทีเพื่อให้ทุกอย่างแสดงได้อย่างถูกต้อง

**เอกสารที่แนะนำ**

- [การโอนความเป็นเจ้าของการสมัครใช้งาน Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [ย้ายทรัพยากรไปยังกลุ่มทรัพยากรใหม่หรือการสมัครใช้งาน](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [จัดการทรัพยากรโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
