---
title: ปัญหาในการเปิดหรือดาวน์โหลดไฟล์ใน Yammer
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
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695668"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>ปัญหาในการเปิดหรือดาวน์โหลดไฟล์ใน Yammer

Yammer คลาสสิกสนับสนุนตัวเลือกหลายตัวเลือกสำหรับการอัปโหลดไฟล์ไปยังข้อความและกลุ่ม โดยขึ้นอยู่กับการกำหนดค่าเครือข่ายไฟล์ค่าเริ่มต้นไปยังที่เก็บข้อมูลใน SharePoint

ตัวใช้เลือกไฟล์ใน Yammer ใหม่ยังไม่สนับสนุนตัวเลือกทั้งหมดที่พร้อมใช้งานใน Yammer แบบคลาสสิก การอัปเดตในอนาคตจะเพิ่มฟีเจอร์เพิ่มเติม สำหรับข้อมูลเพิ่มเติมให้ดูที่[แนบไฟล์หรือรูปภาพลงในโพสต์การสนทนา Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**ไม่สามารถเปิดหรือดาวน์โหลดไฟล์ได้**  

ไฟล์อาจอัปโหลดไปยัง Yammer แต่ยังสามารถเชื่อมโยงไปยังไฟล์ใน SharePoint Online ได้อีกด้วย เมื่อต้องการแก้ไขปัญหาก่อนอื่นคุณจะต้องระบุตำแหน่งที่ตั้งของไฟล์นั้น ถ้าไฟล์ได้รับการอัปโหลดไปยัง Yammer จะมี URL * yammer.com ตรวจสอบให้แน่ใจว่า Url ที่จำเป็นและที่อยู่ IP ไม่ได้รับการบล็อก สำหรับข้อมูลเพิ่มเติมให้ดูที่โพสต์ในบล็อก[โดยใช้ที่อยู่ IP ของรหัสที่ฮาร์สำหรับ Yammer ไม่แนะนำ](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

ตรวจสอบว่าผู้ใช้ที่เป็นผู้ดูแลระบบส่วนกลางสามารถดาวน์โหลดไฟล์ได้หรือไม่ ถ้าไฟล์เป็นแบบส่วนตัวคุณอาจจำเป็นต้องใช้โหมดเนื้อหาส่วนตัว สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ตรวจสอบเนื้อหาส่วนตัวใน Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)  

**ผู้เยี่ยมชมระดับเครือข่าย Yammer และไฟล์ใน SharePoint Online**  

[ผู้เยี่ยมชมระดับเครือข่ายใน Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ไม่ได้ใช้ AZURE AD B2B และอยู่ภายในบริการ Yammer ดังนั้นจึงไม่สามารถเข้าถึงไฟล์ Yammer ที่เก็บไว้ใน SharePoint ได้ สร้างผู้ใช้ B2B ภายนอกที่สามารถเข้าถึงไลบรารีเอกสารใน SharePoint Online โดยใช้ข้อมูลประจำตัวนั้น สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการสนับสนุนของผู้เยี่ยมชมในอนาคตของ Azure AD ใน Yammer ให้ดูที่[การสนับสนุนของผู้เข้าร่วมทางธุรกิจ (B2B) ในการแสดงตัวอย่าง Yammer-ข้อกำหนดและคำถามที่ถามบ่อยของลูกค้า](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)