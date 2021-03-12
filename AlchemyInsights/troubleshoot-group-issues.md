---
title: การแก้ไขปัญหากลุ่ม
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714445"
---
# <a name="troubleshoot-group-issues"></a>การแก้ไขปัญหากลุ่ม

**ฉันต้องการกําหนดกลุ่มให้กับบทบาท Azure AD**

เมื่อต้องการกําหนดกลุ่ม Azure Active Directory (AD) ให้กับบทบาท Azure AD ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. สร้างกลุ่มใหม่ - เมื่อต้องการสร้างกลุ่มใหม่:

    a. ลงชื่อเข้าใช้ศูนย์การจัดการ Azure AD ด้วยสิทธิ์ระดับผู้ดูแลระบบบทบาทที่มีสิทธิ์หรือสิทธิ์ระดับผู้ดูแลระบบส่วนกลาง 
    b. เลือกกลุ่ม azure Active Directory >กลุ่ม>ทั้งหมด>กลุ่มใหม่ 
    c. สร้างกลุ่ม

2. กําหนดบทบาทให้กับกลุ่มระหว่างการสร้างกลุ่มหรือหลังจากสร้างกลุ่ม

    a. เมื่อต้องการกําหนดบทบาทให้กับกลุ่มณ เวลาของการสร้างกลุ่ม คุณสามารถกําหนดบทบาท Azure AD ให้กับกลุ่มและสร้างกลุ่มได้
    b. เมื่อต้องการกําหนดบทบาทให้กับกลุ่มหลังจากสร้างบทบาทแล้ว ให้นําทางไปยังแท็บ บทบาทที่กําหนด ให้กับกลุ่มที่สร้างขึ้นใหม่ และกําหนดบทบาทให้กับกลุ่มนั้น

**ฉันต้องการจัดการการเป็นสมาชิกของกลุ่มที่มอบหมายให้กับบทบาท Azure AD**

1. เมื่อต้องการป้องกันระดับสิทธิ์ ตามค่าเริ่มต้น เฉพาะผู้ดูแลระบบบทบาทที่มีสิทธิ์และผู้ดูแลระบบส่วนกลางเท่านั้นที่สามารถปรับเปลี่ยนการเป็นสมาชิกของกลุ่มที่มอบหมายให้กับบทบาทได้ อย่างไรก็ตาม พวกเขาสามารถเลือกกําหนดเจ้าของให้กับกลุ่มดังกล่าวและมอบสิทธิ์งานนี้ For more information see, [use cloud groups to manage role assignments in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. ดูการแก้ไขปัญหาบทบาทที่กําหนดให้กับกลุ่มใน Azure AD เพื่อดูการแก้ไขปัญหาบทบาทที่กําหนด[ให้กับกลุ่มระบบคลาวด์](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**กลุ่มแบบไดนามิก**

1. ถ้าคุณไม่พบแอตทริบิวต์ผู้ใช้ที่มีอยู่แล้วภายใน ตรวจสอบให้แน่ใจว่าแอตทริบิวต์อยู่ในรายการคุณสมบัติที่สนับสนุน
2. ถ้าคุณค้นหาแอตทริบิวต์ของอุปกรณ์ในตัว ตรวจสอบให้แน่ใจว่าแอตทริบิวต์อยู่ในรายการแอตทริบิวต์ของอุปกรณ์ 
3. นอกเหนือจากแอตทริบิวต์ผู้ใช้และอุปกรณ์ที่มีอยู่แล้วภายใน[คุณยังสามารถใช้แอตทริบิวต์ส่วนขยาย](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) หลังจากซิงค์แอตทริบิวต์ส่วนขยายจาก Windows Server AD ภายในองค์กรหรือจากแอปพลิเคชัน SaaS ที่เชื่อมต่อ แอตทริบิวต์ควรสามารถมองเห็นได้ในรายการดรอปดาวน์ของตัวสร้างกฎ The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name. ซึ่งสามารถใช้ในการสร้างกฎในไวยากรณ์กฎได้
4. ตรวจสอบให้แน่ใจว่าผู้เช่าของคุณมีสิทธิ์การใช้งานที่เหมาะสม กลุ่มแบบไดนามิกต้องการให้ผู้เช่ามีสิทธิ์การใช้งาน Azure AD P1 Premium รายการแผนสิทธิการใช้งาน Azure AD[สามารถเข้าถึงได้ที่นี่](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + แผนการให้สิทธิ์การใช้งาน[ด้านความปลอดภัยสามารถเข้าถึงได้ที่นี่](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. ตรวจสอบให้แน่ใจว่าบทบาทของผู้ใช้ในการสร้างกลุ่มแบบไดนามิกคือผู้ดูแลระบบส่วนกลาง ผู้ดูแลระบบ intun>ผู้ดูแลกลุ่ม หรือผู้ดูแลระบบของผู้ใช้
6. โปรดอนุญาตเวลาสร้างกลุ่ม ขึ้นอยู่กับขนาดของผู้เช่าของคุณ กลุ่มอาจใช้เวลาถึง 24 ชั่วโมงในการเติมข้อมูลเป็นครั้งแรกหรือหลังจากการเปลี่ยนแปลงกฎ
7. For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**ฉันต้องการลบกลุ่ม**

1. กลุ่มอาจถูกลบจากไดเรกทอรีโดยใช้ cmdlet Remove-AzureADGroup cmdlet ในโมดูล Azure AD Powershell
2. ก่อนที่จะพยายามลบกลุ่มที่ซิงค์ใน Azure AD ตรวจสอบให้แน่ใจว่าคุณได้ลบสิทธิ์การใช้งานที่ได้รับมอบหมายทั้งหมดเพื่อหลีกเลี่ยงข้อผิดพลาด
3. For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**ฉันต้องการคืนค่ากลุ่มที่ถูกลบ**

1. ถ้ากลุ่ม Office 365 ถูกลบ กลุ่มจะสามารถคืนค่าได้ภายใน 30 วันก่อนที่มีการลบถาวรเกิดขึ้นเท่านั้น เมื่อลบอย่างถาวร กลุ่มจะไม่สามารถคืนค่าได้อีกต่อไป เรียนรู้เพิ่มเติมเกี่ยวกับการคืนค่า [กลุ่ม](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)ที่นี่
2. หน้าที่การใช้งานนี้ไม่สนับสนุนกลุ่มความปลอดภัยและกลุ่มการแจกจ่าย
3. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้คืนค่ากลุ่ม Office 365 ผู้ดูแลระบบส่วนกลาง ผู้ดูแลระบบกลุ่ม ผู้ดูแลระบบบัญชีผู้ใช้ ผู้ดูแลระบบบริการ intun1 ระดับคู่ค้า หรือการสนับสนุนระดับ2 และเจ้าของกลุ่มสามารถคืนค่ากลุ่มได้
4. เมื่อกลุ่มแบบไดนามิกถูกลบและคืนค่า กลุ่มจะถูกมองเป็นกลุ่มใหม่และสร้างใหม่ตามกฎ ขั้นตอนนี้อาจใช้เวลาถึง 24 ชั่วโมง
5. For more information on restoreing a deleted group, see [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**การกําหนดค่านโยบายการหมดอายุของกลุ่ม**

1. ฟังก์ชันการใช่งานนี้ได้รับการสนับสนุนเฉพาะกลุ่ม Office 365 เท่านั้น และไม่รองรับกลุ่มความปลอดภัยและกลุ่มการแจกจ่าย
2. การกําหนดค่าและการใช้นโยบายการหมดอายุของกลุ่ม Office 365 ต้องใช้สิทธิ์การใช้งาน Azure AD Premium
3. ขณะนี้ คุณสามารถกําหนดค่านโยบายการหมดอายุของกลุ่ม Office 365 บนผู้เช่าได้เพียงนโยบายเดียว
4. เฉพาะผู้ดูแลระบบส่วนกลาง ผู้ดูแลกลุ่ม ผู้ดูแลระบบผู้ใช้ และเจ้าของกลุ่มเท่านั้นที่สามารถต่ออายุกลุ่มได้
5. ถ้ากลุ่ม Office 365 หมดอายุ กลุ่มจะถูกลบและคืนค่าได้ภายใน 30 วันก่อนการลบถาวรเท่านั้น เมื่อลบอย่างถาวร กลุ่มจะไม่สามารถคืนค่าได้อีกต่อไป เรียนรู้เพิ่มเติมเกี่ยวกับการคืนค่า [กลุ่ม](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)ที่นี่

**การต่ออายุอัตโนมัติตามกิจกรรม**

กิจกรรมของผู้ใช้จาก SharePoint, Outlook และ Teams สามารถทริกเกอร์การต่ออายุอัตโนมัติของกลุ่มได้ ตรวจสอบกิจกรรมภายใน 35 วันก่อนที่กลุ่มจะหมดอายุ ถ้ามีกิจกรรมในช่วงวงจรชีวิตกลุ่มปัจจุบัน กลุ่มจะถูกต่ออายุโดยอัตโนมัติและการแจ้งเตือนทางอีเมลจะไม่ถูกส่งออกไปเจ้าของกลุ่ม

**การแจ้งให้ทราบเกี่ยวกับเวลาที่หมดอายุของกลุ่มที่หมดอายุ**

1. การแจ้งเตือนทางอีเมลจะถูกส่งไปยังเจ้าของกลุ่ม Office 365 30 วัน 15 วัน และ 1 วันก่อนที่จะหมดอายุของกลุ่ม
2. เมื่อคุณตั้งค่าวันหมดอายุครั้งแรก กลุ่มใดๆ ที่เก่ากว่าช่วงหมดอายุจะถูกตั้งค่าเป็น 35 วันจนกว่าจะหมดอายุ
3. วันหมดอายุของกลุ่มจะถูกคํานวณโดยยึดตามวันที่ต่ออายุกลุ่ม ไม่ใช่ตามวันที่อัปเดตนโยบาย ถ้ามีการอัปเดตนโยบายวันหมดอายุ วันหมดอายุจะไม่เปลี่ยนแปลง
4. For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and Restore a deleted Office [365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**สิทธิ์ในการสร้างกลุ่ม**

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่ ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัล Azure หรือแผงการเข้าถึง คุณอาจต้องการให้ผู้ดูแลระบบสร้างกลุ่มใหม่ให้คุณ หรือมอบสิทธิ์ที่เหมาะสมให้คุณ

1. [สร้างกลุ่มใหม่และเพิ่มสมาชิกในพอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [สร้างกลุ่มใน Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [ปิดใช้งานการสร้างกลุ่มใน Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [จัดการบุคคลที่สามารถสร้างกลุ่มใน Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [ปิดใช้งานการแจ้งเตือนต้อนรับของ Office 365 ผ่าน Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [บทบาทผู้ดูแลระบบ Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**จัดการสิทธิ์การสร้างกลุ่ม**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การสร้างกลุ่มเพื่อความปลอดภัยหรือกลุ่ม Office 365 ที่สร้างขึ้นในพอร์ทัล Azure หรือแผงการเข้าถึง โดยการตั้งค่าผู้ใช้สามารถสร้างกลุ่มความปลอดภัยใน **พอร์ทัล Azure** หรือผู้ใช้สามารถสร้างกลุ่ม **Office 365** ในการตั้งค่าพอร์ทัล Azure ในกลุ่มทั้งหมด **> ทั่วไป (การตั้งค่า)**
2. คุณยังสามารถจํากัดการสร้างกลุ่มเพื่อเลือกกลุ่มของผู้ใช้ถ้าคุณมีสิทธิ์การใช้งาน Azure AD P1 Premium

**การปิดใช้งานการแจ้งเตือนต้อนรับให้กับสมาชิกใหม่ในกลุ่ม Office 365**

สามารถปิดใช้งานการแจ้งเตือนต้อนรับที่ส่งถึงผู้ใช้ที่ถูกเพิ่มลงในกลุ่ม Office 365 ได้ด้วย `UnifiedGroupWelcomeMessageEnabled` การตั้งค่าเป็น **False** ใน Powershell เรียนรู้เกี่ยวกับการตั้งค่า [นี้](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)ได้ที่นี่













