---
title: ปัญหาการเปิดหรือดาวน์โหลดแฟ้มใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148436"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>ปัญหาการเปิดหรือดาวน์โหลดแฟ้มใน Yammer

Yammer แบบคลาสสิกสนับสนุนตัวเลือกหลายตัวเลือกสําหรับการอัปโหลดแฟ้มไปยังข้อความและกลุ่ม แฟ้มเริ่มต้นสําหรับที่เก็บข้อมูลใน SharePoint ขึ้นอยู่กับการกําหนดค่าเครือข่าย

ตัวเลือกแฟ้มใน Yammer ใหม่ไม่สนับสนุนตัวเลือกทั้งหมดที่มีอยู่ใน Yammer แบบคลาสสิก การปรับปรุงในอนาคตจะเพิ่มคุณลักษณะเพิ่มเติม สําหรับข้อมูลเพิ่มเติม ให้ดูที่[แนบไฟล์หรือรูปภาพลงในโพสต์สนทนา Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**ไม่สามารถเปิดหรือดาวน์โหลดแฟ้ม**  

แฟ้มอาจอัปโหลดไปยัง Yammer แต่ยังเชื่อมโยงไปยังแฟ้มใน SharePoint แบบออนไลน์ เมื่อต้องการแก้ไขปัญหา ก่อนอื่นคุณต้องกําหนดตําแหน่งที่ตั้งของแฟ้ม ถ้าแฟ้มถูกอัปโหลดไปยัง Yammer แฟ้มนั้นจะมี URL *.yammer.com ตรวจสอบให้แน่ใจว่า URL และที่อยู่ IP ที่ต้องการถูกยกเลิกการบล็อก สําหรับข้อมูลเพิ่มเติม[ให้ดูที่โพสต์บล็อก](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

ตรวจสอบว่าผู้ใช้ที่เป็นผู้ดูแลระบบส่วนกลางสามารถดาวน์โหลดไฟล์ได้หรือไม่ ถ้าแฟ้มเป็นส่วนตัว คุณอาจต้องใช้โหมดเนื้อหาส่วนตัว สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตรวจสอบเนื้อหาส่วนตัวใน Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)  

**ผู้ใช้และแฟ้มระดับเครือข่าย Yammer ใน SharePoint แบบออนไลน์**  

[ผู้ใช้ระดับเครือข่ายใน Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)ไม่ได้ใช้ Azure AD B2B และภายในไปยังบริการ Yammer ดังนั้นพวกเขาจึงไม่สามารถเข้าถึงแฟ้ม Yammer ที่เก็บไว้ใน SharePoint สร้างผู้ใช้ AAD B2B ภายนอกที่สามารถเข้าถึงไลบรารีเอกสารใน SharePoint แบบออนไลน์ โดยใช้ข้อมูลประจําตัวนั้น สําหรับข้อมูลเกี่ยวกับการสนับสนุนผู้เยี่ยมชม Azure AD B2B ในอนาคตใน Yammer ให้ดูที่[การสนับสนุนผู้เยี่ยมชมธุรกิจ (B2B) ใน Yammer Preview - ข้อกําหนดของลูกค้าและคําถามที่ถามบ่อย](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)