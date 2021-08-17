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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109223"
---
# <a name="save-site-or-list-as-a-template"></a>บันทึกไซต์หรือรายการเป็นเทมเพลต

SharePointไซต์ของคุณคือความหมายที่สร้างไว้ล่วงหน้าซึ่งได้รับการออกแบบมาเฉพาะความต้องการทางธุรกิจบางอย่าง For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

ต่อไปนี้คือปัญหา/วิธีแก้ไขปัญหาทั่วไปเกี่ยวกับการบันทึกไซต์หรือรายการเป็นเทมเพลตใน SharePoint Online

**ปุ่ม บันทึกเทมเพลตไซต์/รายการ ไม่พร้อมใช้งานหรือ** ขาดหายไป 

- ผู้ดูแลระบบจะต้อง อนุญาตสคริปต์แบบปรับแต่งเอง เพื่อเปิดใช้งานฟีเจอร์เทมเพลต For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- ไม่สนับสนุนการสั่ง บันทึกไซต์เป็นเทมเพลต และอาจทําให้เกิดปัญหาบนไซต์ที่ใช้โครงสร้างพื้นฐาน SharePoint Server Publishing ได้


**ไม่สามารถสร้างเทมเพลตไซต์ได้ หรือไม่สามารถใช้งานได้อย่างถูกต้อง**

- เทมเพลตอาจไม่มี [ฟีเจอร์](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) และจะไม่เปิดใช้งาน ถ้าฟีเจอร์นี้ไม่สามารถเปิดใช้งานในไซต์คอลเลกชันปัจจุบันได้ คุณจะไม่สามารถใช้เทมเพลตไซต์เพื่อสร้างไซต์ได้


- ตรวจสอบเพื่อดูว่ามีรายการหรือไลบรารีใดๆ [เกินค่าเกณฑ์](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ขีดจํากัดของมุมมองรายการ 5000 รายการหรือไม่ เนื่องจากสามารถบล็อกการสร้างเทมเพลตไซต์ได้


- ไซต์อาจใช้ทรัพยากรมากเกินไป ดังนั้น เทมเพลตไซต์จึงเกินขีดจํากัด 50 เมกะไบต์ (MB)


- มีปัญหาในการแสดงข้อมูลจากรายการที่ใช้คอลัมน์ค้นหา For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

