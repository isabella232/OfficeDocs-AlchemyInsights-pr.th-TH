---
title: ปัญหาในการเปิดหรือดาวน์โหลดไฟล์ในYammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028275"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>ปัญหาในการเปิดหรือดาวน์โหลดไฟล์ในYammer

ตัวเลือกYammerรองรับการอัปโหลดไฟล์ไปยังข้อความและกลุ่มได้หลายตัวเลือก ขึ้นอยู่กับการกําหนดค่าเครือข่าย ไฟล์จะเป็นค่าเริ่มต้นของที่SharePoint

ตัวเลือกไฟล์ในตัวเลือกYammerยังไม่สนับสนุนตัวเลือกทั้งหมดที่พร้อมใช้งานในรุ่นYammer การอัปเดตในอนาคตจะเพิ่มฟีเจอร์เพิ่มเติม ดูข้อมูลเพิ่มเติมได้ที่ แนบ[ไฟล์หรือรูปภาพลงในYammerโพสต์การสนทนา](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**ไม่สามารถเปิดหรือดาวน์โหลดไฟล์ได้**  

ไฟล์อาจอัปโหลดYammerไปยังไฟล์ แต่ยังลิงก์ไปยังไฟล์ใน SharePoint Online ด้วย เมื่อต้องการแก้ไขปัญหา ก่อนอื่นคุณต้องระบุที่ตั้งของไฟล์ ถ้าไฟล์ถูกอัปโหลดYammer ไฟล์จะมี *.yammer.com URL ตรวจสอบให้แน่ใจว่า URL และที่อยู่ IP ที่ต้องใช้ยกเลิกการบล็อกแล้ว For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

ตรวจสอบว่าผู้ใช้ที่เป็นผู้ดูแลระบบส่วนกลางสามารถดาวน์โหลดไฟล์ได้หรือไม่ ถ้าไฟล์เป็นแบบส่วนตัว คุณอาจต้องใช้โหมดเนื้อหาส่วนตัว ดูข้อมูลเพิ่มเติมได้ที่ จากนั้น ตรวจสอบ[เนื้อหาส่วนตัวใน Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)  

**Yammerและไฟล์ระดับเครือข่ายใน SharePoint Online**  

[ผู้ใช้ภายนอกระดับเครือข่ายใน Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)อย่าใช้ Azure AD B2B และอยู่ในบริการ Yammer ดังนั้น พวกเขาไม่สามารถเข้าถึงไฟล์Yammerที่SharePointได้ สร้างผู้ใช้ AAD B2B ภายนอกที่สามารถเข้าถึงไลบรารีเอกสารใน SharePoint Online โดยใช้ข้อมูลเฉพาะตัวนั้น For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).