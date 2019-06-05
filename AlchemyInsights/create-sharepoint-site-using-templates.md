---
title: สร้างไซต์ใน SharePoint แบบออนไลน์
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 2097933dd20f326a7bda2151596d514c37d566ff
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717785"
---
# <a name="create-sharepoint-sites-using-templates"></a>สร้างไซต์ SharePoint โดยใช้แม่แบบ

แม่แบบไซต์ SharePoint จะปรากฏคำนิยามที่ออกแบบมาให้อยู่รอบ ๆ ความต้องการเฉพาะทางด้านธุรกิจ สำหรับข้อมูลเพิ่มเติม ดู<a href="https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4">โดยใช้แม่แบบเพื่อสร้างชนิดของไซต์ SharePoint</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ต่อไปนี้เป็นปัญหา/แก้ไขปัญหาทั่วไปบางอย่างเกี่ยวกับการบันทึกเป็นไซต์หรือรายการเป็นแม่แบบใน Sharepoint แบบออนไลน์</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">บันทึกลงรายการไซต์แม่แบบปุ่มจะไม่พร้อมใช้งาน หรือหายไป</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ผู้ดูแลจะต้องใช้เมื่อต้องการอนุญาตให้ใช้สคริปต์แบบกำหนดเองเพื่อเปิดใช้งานลักษณะการทำงานของแม่แบบ สำหรับขั้นตอนโดยละเอียด ตัวอย่าง และข้อควรพิจารณาดู</span> </span><a style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">อนุญาต หรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง</a></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ไซต์บันทึกแม่แบบในคำสั่งไม่ได้รับการสนับสนุน และอาจทำให้เกิดปัญหาบนไซต์ที่ใช้ SharePoint Server ประกาศโครงสร้างพื้นฐาน</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">แม่แบบไซต์ไม่สามารถสร้าง หรือทำงานไม่ถูกต้อง</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">แม่แบบอาจไม่มี<a href="https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx">คุณลักษณะ</a>และชนะ&rsquo;t ที่เรียกใช้งานได้ ถ้าคุณลักษณะนี้ไม่พร้อมใช้งานเพื่อเรียกใช้งานในไซต์คอลเลกชันปัจจุบัน คุณไม่สามารถใช้แม่แบบไซต์เพื่อสร้างไซต์</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ตรวจสอบถ้ารายการหรือไลบรารีใด ๆ เกิน<a href="https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59">ขีดจำกัดการจำกัดมุมมองรายการของ</a>5000 รายการขณะนี้สามารถบล็อคการสร้างแม่แบบไซต์หรือไม่</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ไซต์อาจจะกำลังใช้ทรัพยากรมากเกินไป และดังนั้น แม่แบบไซต์เกินขีดจำกัด 50 MB</span></li> <li>
มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์ค้นหา สำหรับข้อมูลเพิ่มเติม</span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> <a style="box-sizing: border-box; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a"><span style="color: #0067b8; text-decoration: none; text-underline: none;">การสร้างแม่แบบรายการ&rsquo;ข้อมูลแสดง t จากรายการการค้นหาที่ถูกต้องใน SharePoint แบบออนไลน์

สำหรับข้อมูลเกี่ยวกับปัญหาและวิธีแก้ไขปัญหาทั่วไปรายละเอียดเพิ่มเติม โปรดตรวจสอบ<a href="https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989">สร้างและใช้แม่แบบไซต์



