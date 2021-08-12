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
ms.openlocfilehash: 47f00118a5a4b446b6a3b06f0fc6101d00d11b626eaf249bb6ca962a55f7f4d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939362"
---
# <a name="troubleshoot-group-issues"></a>การแก้ไขปัญหากลุ่ม

**ฉันต้องการกําหนดกลุ่มให้กับบทบาท Azure AD**

เมื่อต้องการมอบหมายกลุ่มAzure Active Directory (AD) ให้กับบทบาท Azure AD ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. สร้างกลุ่มใหม่ - เมื่อต้องการสร้างกลุ่มใหม่:

    a. ลงชื่อเข้าใช้ศูนย์การจัดการ Azure AD ด้วยผู้ดูแลระบบบทบาทที่มีสิทธิ์พิเศษหรือสิทธิ์ระดับผู้ดูแลระบบส่วนกลาง 
    b. เลือก Azure Active Directory >กลุ่ม> กลุ่มทั้งหมด > กลุ่มใหม่ 
    c. สร้างกลุ่ม

2. กําหนดบทบาทให้กับกลุ่มระหว่างการสร้างกลุ่มหรือหลังจากสร้างกลุ่ม

    a. เมื่อต้องการกําหนดบทบาทให้กับกลุ่มณ เวลาของการสร้างกลุ่ม คุณสามารถกําหนดบทบาท Azure AD ให้กับกลุ่มและสร้างกลุ่มได้
    b. เมื่อต้องการกําหนดบทบาทให้กับกลุ่มหลังจากสร้างบทบาทแล้ว ให้นําทางไปยังแท็บ บทบาทที่มอบหมาย ของกลุ่มที่สร้างขึ้นใหม่ และกําหนดบทบาทให้กับกลุ่มนั้น

**ฉันต้องจัดการการเป็นสมาชิกของกลุ่มที่มอบหมายให้กับบทบาท Azure AD**

1. เมื่อต้องการป้องกันระดับสิทธิ์ ตามค่าเริ่มต้น เฉพาะผู้ดูแลระบบบทบาทที่มีสิทธิ์พิเศษและผู้ดูแลระบบส่วนกลางเท่านั้นที่สามารถปรับเปลี่ยนการเป็นสมาชิกของกลุ่มที่มอบหมายให้กับบทบาทได้ อย่างไรก็ตาม พวกเขาสามารถเลือกกําหนดเจ้าของให้กับกลุ่มดังกล่าวและมอบหมายงานนี้ให้ผู้รับมอบสิทธิ์ ดูข้อมูลเพิ่มเติมที่[ใช้กลุ่มระบบคลาวด์เพื่อจัดการการมอบหมายบทบาทAzure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. ดูข้อสงสัยทั่วไปและเคล็ดลับการแก้ไขปัญหาการกําหนดบทบาทให้กับกลุ่มใน Azure AD ดู [การแก้ไขปัญหาบทบาทที่กําหนดให้กับกลุ่ม](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)ระบบคลาวด์

**กลุ่มแบบไดนามิก**

1. ถ้าคุณไม่พบแอตทริบิวต์ผู้ใช้ที่มีอยู่แล้วภายใน ให้ตรวจสอบว่าแอตทริบิวต์อยู่ในรายการของคุณสมบัติที่สนับสนุน
2. ถ้าคุณค้นหาแอตทริบิวต์ของอุปกรณ์ที่มีอยู่แล้วภายใน ตรวจสอบให้แน่ใจว่าแอตทริบิวต์อยู่ในรายการแอตทริบิวต์ของอุปกรณ์ 
3. นอกเหนือจากแอตทริบิวต์ของผู้ใช้และแอตทริบิวต์อุปกรณ์ที่มีอยู่แล้วภายใน คุณยังสามารถใช้แอตทริบิวต์ [ส่วนขยาย](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)ได้ หลังจากซิงค์แอตทริบิวต์ส่วนขยายจากภายในองค์กร Windows Server AD หรือจากแอปพลิเคชัน SaaS ที่เชื่อมต่อแอตทริบิวต์ควรสามารถมองเห็นได้ในรายการดรอปดาวน์ของตัวสร้างกฎ The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name. These could also be used when constructing rules in the rule syntax.
4. ตรวจสอบให้แน่ใจว่าผู้เช่าของคุณมีสิทธิ์การใช้งานที่เหมาะสม กลุ่มแบบไดนามิกต้องการผู้เช่าเพื่อให้มีสิทธิ์การใช้งาน Azure AD P1 Premiumได้ รายการแผนสิทธิการใช้งาน Azure AD[สามารถเข้าถึงได้ที่นี่](https://azure.microsoft.com/pricing/details/active-directory/) สามารถเข้าถึงแผน Enterprise Mobility + Security [Licensing](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)ได้ที่นี่
5. ตรวจสอบให้แน่ใจว่าบทบาทของผู้ใช้ในการสร้างกลุ่มแบบไดนามิกคือผู้ดูแลระบบส่วนกลาง ผู้ดูแลระบบ Intuns ผู้ดูแลกลุ่ม หรือผู้ดูแลระบบผู้ใช้
6. โปรดอนุญาตให้กลุ่มสร้างข้อมูล ขึ้นอยู่กับขนาดของผู้เช่าของคุณ กลุ่มอาจใช้เวลาถึง 24 ชั่วโมงในการเติมข้อมูลเป็นครั้งแรกหรือหลังจากการเปลี่ยนแปลงกฎ
7. For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**ฉันต้องการลบกลุ่ม**

1. กลุ่มสามารถถูกลบจากไดเรกทอรีโดยใช้ cmdlet Remove-AzureADGroupในมอดูล Azure AD Powershell
2. ก่อนที่จะพยายามลบกลุ่มที่ซิงค์ใน Azure AD ตรวจสอบให้แน่ใจว่าคุณได้ลบสิทธิ์การใช้งานที่ได้รับมอบหมายทั้งหมดเพื่อหลีกเลี่ยงข้อผิดพลาด
3. For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**ฉันต้องการคืนค่ากลุ่มที่ถูกลบ**

1. ถ้ากลุ่มOffice 365ลบ กลุ่มดังกล่าวจะสามารถคืนค่าได้ภายใน 30 วันก่อนที่การลบถาวรจะเกิดขึ้นเท่านั้น เมื่อลบอย่างถาวร กลุ่มจะไม่สามารถคืนค่าได้อีกต่อไป เรียนรู้เพิ่มเติมเกี่ยวกับการคืนค่า [กลุ่ม](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)ที่นี่
2. ฟังก์ชันการรักษาความปลอดภัยและกลุ่มการแจกจ่ายไม่ได้รับการสนับสนุน
3. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้คืนค่ากลุ่มOffice 365ของคุณ ผู้ดูแลระบบส่วนกลาง ผู้ดูแลระบบกลุ่ม ผู้ดูแลระบบบัญชีผู้ใช้ ผู้ดูแลระบบบริการ Intunอีเมล ระดับคู่ค้าระดับ1 หรือการสนับสนุน Tier2 และเจ้าของกลุ่มสามารถคืนค่ากลุ่มได้
4. เมื่อกลุ่มแบบไดนามิกถูกลบและคืนค่า กลุ่มจะถูกมองเป็นกลุ่มใหม่และเติมข้อมูลใหม่ตามกฎ ขั้นตอนนี้อาจใช้เวลาถึง 24 ชั่วโมง
5. หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับการคืนค่ากลุ่มที่ถูกลบ ให้ดู[คืนค่ากลุ่มOffice 365ที่ถูกลบใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**การกําหนดค่านโยบายการหมดอายุของกลุ่ม**

1. ฟังก์ชันการฟังก์ชันนี้Office 365กลุ่มการแจกจ่ายเท่านั้น และไม่รองรับกลุ่มความปลอดภัยและกลุ่มการแจกจ่าย
2. การกําหนดค่าและการใช้นโยบายวันหมดอายุOffice 365กลุ่มของคุณต้องมีสิทธิ์การใช้งาน Azure AD Premiumเหล่านี้
3. ขณะนี้ สามารถกําหนดค่านโยบายวันหมดอายุได้เพียงOffice 365กลุ่มเดียวในผู้เช่า
4. เฉพาะผู้ดูแลระบบส่วนกลาง ผู้ดูแลกลุ่ม ผู้ดูแลระบบผู้ใช้ และเจ้าของกลุ่มเท่านั้นที่สามารถต่ออายุกลุ่มได้
5. ถ้ากลุ่มOffice 365หมดอายุ กลุ่มนั้นจะถูกลบและสามารถคืนค่าได้ภายใน 30 วันก่อนที่การลบถาวรจะเกิดขึ้นเท่านั้น เมื่อลบอย่างถาวร กลุ่มจะไม่สามารถคืนค่าได้อีกต่อไป เรียนรู้เพิ่มเติมเกี่ยวกับการคืนค่า [กลุ่ม](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)ที่นี่

**การต่ออายุอัตโนมัติตามกิจกรรม**

กิจกรรมของผู้ใช้ตั้งแต่ SharePoint OutlookและTeamsกลุ่มการต่ออายุอัตโนมัติได้ กิจกรรมจะถูกตรวจสอบภายใน 35 วันก่อนที่กลุ่มจะหมดอายุ ถ้ามีกิจกรรมในช่วงวงจรชีวิตกลุ่มปัจจุบัน กลุ่มจะถูกต่ออายุโดยอัตโนมัติและการแจ้งเตือนทางอีเมลจะไม่ถูกส่งไปยังเจ้าของกลุ่ม

**การตั้งเวลาการแจ้งเตือนของกลุ่มที่หมดอายุ**

1. การแจ้งเตือนทางอีเมลจะถูกส่งไปยังเจ้าของOffice 365 30 วัน, 15 วัน และ 1 วันก่อนหมดอายุของกลุ่ม
2. เมื่อคุณตั้งค่าวันหมดอายุครั้งแรก กลุ่มใดๆ ที่เก่ากว่าช่วงหมดอายุจะถูกตั้งค่าเป็น 35 วันจนกว่าจะหมดอายุ
3. วันหมดอายุของกลุ่มจะถูกคํานวณโดยยึดตามวันที่ต่ออายุของกลุ่ม โดยจะไม่ยึดตามวันที่ที่อัปเดตนโยบาย ถ้านโยบายหมดอายุได้รับการอัปเดต วันหมดอายุจะไม่เปลี่ยนแปลง
4. For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and Restore a deleted Office 365 group in [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**สิทธิ์ในการสร้างกลุ่ม**

ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างกลุ่มใหม่ ผู้ดูแลระบบส่วนกลางสามารถปิดใช้งานการสร้างกลุ่มในพอร์ทัล Azure หรือแผงการเข้าถึงได้ คุณอาจต้องใช้ผู้ดูแลระบบเพื่อสร้างกลุ่มใหม่ให้คุณ หรือมอบสิทธิ์ที่เหมาะสมแก่คุณ

1. [สร้างกลุ่มใหม่และเพิ่มสมาชิกในพอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [สร้างกลุ่มใน Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [ปิดใช้งานการสร้างกลุ่มใน Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [จัดการบุคคลที่สามารถสร้างกลุ่มใน Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [ปิดใช้งานOffice 365ต้อนรับผ่านทาง Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [บทบาทผู้ดูแลระบบ Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**จัดการสิทธิ์การสร้างกลุ่ม**

1. ผู้ดูแลระบบส่วนกลางสามารถจัดการสิทธิ์การสร้างกลุ่มเพื่อความปลอดภัยหรือกลุ่ม Office 365 ที่สร้างขึ้นในพอร์ทัล Azure หรือแผงการเข้าถึง โดยการตั้งค่า ผู้ใช้สามารถสร้างกลุ่มความปลอดภัยในพอร์ทัล **Azure** หรือผู้ใช้สามารถสร้างกลุ่ม **Office 365 ในการตั้งค่า** พอร์ทัล Azure ใน กลุ่มทั้งหมด **> ทั่วไป (การตั้งค่า)**
2. คุณยังสามารถจํากัดการสร้างกลุ่มเพื่อเลือกกลุ่มของผู้ใช้ ถ้าคุณมีสิทธิ์การใช้งาน Azure AD P1 Premium

**การปิดใช้งานการแจ้งเตือนต้อนรับของสมาชิกใหม่Office 365กลุ่ม**

การแจ้งเตือนต้อนรับที่ส่งถึงผู้ใช้ที่ถูกเพิ่มลงในกลุ่มOffice 365ถูกปิดใช้งานโดยการตั้งค่า `UnifiedGroupWelcomeMessageEnabled` **เป็น False** ใน Powershell เรียนรู้เกี่ยวกับการตั้งค่า [นี้](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)ที่นี่













