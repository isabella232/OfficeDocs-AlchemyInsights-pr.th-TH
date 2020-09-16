---
title: การแก้ไขปัญหาประสิทธิภาพการทำงานของ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757904"
---
# <a name="troubleshoot-onedrive-performance"></a>การแก้ไขปัญหาประสิทธิภาพการทำงานของ OneDrive

ถ้าคุณพบว่าการซิงค์ที่คาดว่าจะทำงานช้ากว่าหรือปัญหาประสิทธิภาพการทำงานที่คล้ายคลึงกันกับ OneDrive ให้ทำดังนี้

- ยืนยันว่าไม่มีปัญหาที่ทราบแล้วโดยใช้[แดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth)

- [เปิดใช้งานไฟล์ตามความต้อง](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) การเพื่อให้คุณสามารถเข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive ได้โดยไม่ต้องดาวน์โหลดทั้งหมดและใช้พื้นที่เก็บข้อมูลบนอุปกรณ์ของคุณ

- [ตรวจทานแนวทางปฏิบัติที่ดีที่สุด](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) สำหรับการวางแผนเครือข่ายและประสิทธิภาพการทำงาน

- [เพิ่มความเร็วในการอัปโหลดและดาวน์โหลด](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)โดยเฉพาะอย่างยิ่งถ้าคุณกำลังซิงค์อุปกรณ์เป็นครั้งแรก

- ถ้าคุณกำลังซิงค์ไลบรารีที่มีรายการมากกว่า๑๐๐,๐๐๐รายการการซิงค์ OneDrive อาจดูเหมือนเป็นเวลานานหรือสถานะแสดงการประมวลผล0KB ของ xMB [เรียนรู้เพิ่มเติมเกี่ยวกับการซิงค์ไฟล์มากกว่า๑๐๐,๐๐๐](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)และ[การจำกัดจำนวนไฟล์๓๐๐,๐๐๐ที่ได้รับการสนับสนุนของ OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)

- เมื่อผู้ใช้เกินขีดจำกัดการใช้งาน SharePoint Online throttles การร้องขอเพิ่มเติมใดๆจากบัญชีผู้ใช้นั้นเป็นระยะเวลาสั้นๆ การกระทำของผู้ใช้ทั้งหมดจะปริมาณขณะที่เค้นอยู่ในลักษณะพิเศษ
