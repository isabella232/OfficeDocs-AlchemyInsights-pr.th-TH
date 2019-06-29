---
title: การแก้ไขปัญหาประสิทธิภาพการทำงานของ OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: a78ef48aa92cbcfa27f14aa755e4810e410dddc1
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367256"
---
# <a name="troubleshoot-onedrive-performance"></a>การแก้ไขปัญหาประสิทธิภาพการทำงานของ OneDrive

ถ้าคุณประสบกับช้ากว่าการซิงค์ที่คาดไว้ หรือปัญหาเกี่ยวกับประสิทธิภาพการทำงานคล้ายกับ OneDrive:

- ยืนยันว่า จะไม่มีปัญหาที่ทราบที่ใช้[แดชบอร์ดสถานภาพการบริการ](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fportal.office.com%2Fadminportal%2Fhome%23%2Fservicehealth&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051385661&sdata=z3OU7adaVjJorTGK8v7Ipo35E5vkk35lVCEzgGYQoNo%3D&reserved=0)

- [เปิดใช้งานแฟ้มในความต้องการ](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fsave-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051395670&sdata=QN1F4v1q6pNV2hIZ5LCZTtIbuv%2FR7lH5C5g%2FAFJQhrM%3D&reserved=0)เพื่อให้คุณสามารถเข้าถึงแฟ้มของคุณทั้งหมดใน OneDrive ได้ โดยไม่ต้องดาวน์โหลดทั้งหมด และใช้เนื้อที่เก็บข้อมูลบนอุปกรณ์ของคุณ

- [ทบทวนแนวทางปฏิบัติที่ดีที่สุด](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Foffice365%2Fenterprise%2Fnetwork-planning-and-performance&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=RQCPPj7XPAm4IK6jKf1xugHnxXqqJoKK%2BlEENg7WrDQ%3D&reserved=0)สำหรับการวางแผนเครือข่ายและประสิทธิภาพการทำงาน

- [ขยายใหญ่สุดที่อัปโหลด และดาวน์โหลดเร็ว](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FMaximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=vR4z9GSeObeKY3ouE7oru4Vr%2FGn%2FghUoFBjpRQbfvhA%3D&reserved=0)โดยเฉพาะอย่างยิ่งถ้าคุณกำลังทำการซิงค์กับอุปกรณ์เป็นครั้งแรกเท่านั้น

- ถ้าคุณกำลังซิงค์ไลบรารีกับสินค้ามากกว่า 100000 ซิงค์ OneDrive อาจดูเหมือนยังติดอยู่เป็นเวลานาน หรือแสดงสถานะการประมวลผล 0 KB ของ xMB " [เรียนรู้เพิ่มเติมเกี่ยวกับการซิงค์แฟ้มมากกว่า 100000](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23synctoomany&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051415686&sdata=E4zeoBeRBnlGB1haZXTy%2FJfXMBWSPZCbp6JQvt5qX2o%3D&reserved=0)ตลอดจน[วงเงินสนับสนุนของ OneDrive ของแฟ้ม 300,000](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23numberitemscanbesynced&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051425695&sdata=uqBKB3ykz9QDOPRmSf5YIKBUiNa57IdQVzeLZWL%2BMWc%3D&reserved=0)

- เมื่อผู้ใช้เกินขีดจำกัดการใช้งาน SharePoint ออนไลน์ throttles คำขอเพิ่มเติมใด ๆ จากบัญชีผู้ใช้นั้นในระยะสั้น ๆ การกระทำของผู้ใช้ทั้งหมดจะถูกควบคุมปริมาณในขณะที่ดำเนินการมีผลบังคับ
