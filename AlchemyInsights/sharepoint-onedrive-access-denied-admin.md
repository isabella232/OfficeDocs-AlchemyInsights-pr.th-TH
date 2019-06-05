---
title: การแก้ไขปัญหาข้อความที่มีการเข้าถึงถูกปฏิเสธ
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716665"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>การแก้ไขปัญหาการเข้าถึงถูกปฏิเสธข้อความในศูนย์กลางการดูแล Sharepoint/OneDrive

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">หากคุณได้รับการเข้าถึงถูกปฏิเสธข้อความเมื่อคุณพยายามเรียกดูไปยังศูนย์ดูแล Sharepoint/OneDrive โปรดตรวจสอบให้แน่ใจว่าคุณ<a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">มอบหมายสิทธิ์ให้กับผู้ใช้</a> ถ้าผู้ใช้มีสิทธิ์การใช้งาน คุณควรทำแน่ใจว่า<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">กำหนดบทบาทเป็นผู้ดูแลระบบ</a>ที่สามารถเข้าถึงศูนย์การดูแลด้วย</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">ปัญหานี้สามารถเกิดขึ้นเมื่อผู้ใช้ถูกลบออก และสร้างขึ้นใหม่ ด้วยชื่อเดียวกันผู้ใช้หลัก (UPN) สร้างบัญชีใหม่ โดยใช้ค่า PUID (ID เฉพาะของ Passport) แตกต่างกัน เมื่อผู้ใช้พยายามเข้าถึงไซต์คอลเลกชันหรือ OneDrive ของพวกเขา ผู้ใช้มี PUID ที่ไม่ถูกต้อง สถานการณ์สมมติที่สองเกี่ยวข้องกับไดเรกทอรีการซิงโครไนส์กับ Active Directory หน่วยองค์กร (OU) ถ้าผู้ใช้มีอยู่แล้วลงชื่อเข้าใช้ SharePoint แล้วจะถูกย้ายไปยัง OU อื่น และ resynced กับ SharePoint พวกเขาอาจพบปัญหานี้</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">เมื่อต้องการแก้ไขปัญหานี้ คุณควรคืนค่า UPN เดิม ด้วยขั้นตอนต่าง ๆ ในบทความ<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">การคืนค่าผู้ใช้ใน Office 365</a></span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">หมายเหตุ:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">ถ้าเป็นศูนย์ OneDrive หรือผู้ดูแล SharePoint ไม่พร้อมใช้งานสำหรับผู้ใช้หลายคนที่มีการเข้าถึงไว้ก่อนหน้านี้ อาจมีปัญหาการบริการชั่วคราวได้&nbsp;</span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"><a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">ตรวจสอบแดชบอร์ความสมบูรณ์ของการบริการ</span></a></span></em></span></span></p>


