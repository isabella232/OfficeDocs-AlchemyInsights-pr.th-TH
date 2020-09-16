---
title: บันทึกไซต์หรือรายการเป็นเทมเพลต
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727550"
---
# <a name="save-site-or-list-as-a-template"></a>บันทึกไซต์หรือรายการเป็นเทมเพลต

เทมเพลตของไซต์ SharePoint คือข้อกำหนดสร้างไว้ล่วงที่ได้รับการออกแบบรอบๆความต้องการทางธุรกิจที่เฉพาะเจาะจง สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การใช้เทมเพลตเพื่อสร้างไซต์ SharePoint ชนิดต่างๆ](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

ต่อไปนี้เป็นปัญหาทั่วไป/วิธีแก้ไขปัญหาทั่วไปเกี่ยวกับการบันทึกไซต์หรือรายการเป็นเทมเพลตใน SharePoint Online

**ปุ่มบันทึกเทมเพลตไซต์/รายการจะไม่พร้อมใช้งานหรือหายไป** 

- ผู้ดูแลระบบจะต้องเปิดใช้งานสคริปต์แบบกำหนดเองเพื่อเปิดใช้งานฟีเจอร์เทมเพลต สำหรับขั้นตอนโดยละเอียดตัวอย่างและข้อควรพิจารณาในการ[อนุญาตหรือป้องกันไม่ให้สคริปต์แบบกำหนดเอง](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- คำสั่งบันทึกไซต์เป็นเทมเพลตจะไม่ได้รับการสนับสนุนและอาจทำให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐานของการประกาศของ SharePoint Server


**ไม่สามารถสร้างเทมเพลตของไซต์หรือทำงานได้อย่างถูกต้อง**

- เทมเพลตนี้อาจไม่มี [ฟีเจอร์](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) และไม่สามารถเปิดใช้งานได้ ถ้าฟีเจอร์ไม่พร้อมใช้งานเมื่อต้องการเปิดใช้งานในไซต์คอลเลกชันปัจจุบันคุณจะไม่สามารถใช้เทมเพลตของไซต์เพื่อสร้างไซต์ได้


- ตรวจสอบดูว่ารายการหรือไลบรารีใดที่เกินขีด [จำกัดของมุมมองรายการ](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ของรายการ๕๐๐๐เนื่องจากการทำเช่นนี้สามารถบล็อกการสร้างเทมเพลตของไซต์ได้


- ไซต์อาจใช้แหล่งข้อมูลมากเกินไปและดังนั้นแม่แบบไซต์เกินขีดจำกัด๕๐เมกะไบต์ (MB)


- มีปัญหาเกิดขึ้นในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์การค้นหา สำหรับข้อมูลเพิ่มเติมให้ดูที่[รายการที่สร้างขึ้นโดยใช้เทมเพลตไม่แสดงข้อมูลจากรายการการค้นหาที่ถูกต้องใน SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


สำหรับข้อมูลรายละเอียดเพิ่มเติมเกี่ยวกับปัญหาทั่วไปและการแก้ไขปัญหาโปรดอ้างอิง[สร้างและใช้เทมเพลตของไซต์](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

