---
title: ลบรายการใน SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: af5691d7-a55f-4ece-90c8-d6aaece66b1c
ms.openlocfilehash: 6edc109d2a2f6ec899243fc30d3b9d91d3996c7e
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719990"
---
# <a name="restore-items-deleted-from-sharepoint"></a>เรียกคืนรายการที่ถูกลบออกจาก SharePoint

เมื่อคุณลบสินค้าหรือไซต์จาก Sharepoint จะไม่ได้เสียบ&rsquo;t ทันทีเอาออก รายการที่ถูกลบไปไว้ในถังรีไซเคิลสำหรับรอบระยะเวลา ในช่วงเวลานั้น คุณสามารถคืนค่ารายการคุณลบไปตำแหน่งที่ตั้งเดิม สำหรับข้อมูลเพิ่มเติม โปรดเยี่ยมชมลิงค์ด้านล่าง</p> <p><strong>คืนค่าแฟ้มที่ถูกลบ โฟลเดอร์ และไซต์จากถังรีไซเคิล</strong></p> <ul> <li style="font-weight: 400;"><a href="https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US">คืนค่ารายการในถังรีไซเคิลของไซต์ SharePoint</a></li> </ul> <ul> <li style="font-weight: 400;"><a href="https://support.office.com/en-us/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f">ลบการคืนค่าแฟ้มหรือโฟลเดอร์ใน OneDrive</a></li> </ul> <ul> <li style="font-weight: 400;"><a href="https://docs.microsoft.com/sharepoint/restore-deleted-site-collection">คืนค่าลบไซต์คอลเลกชัน (รวมทั้งกลุ่ม การสื่อสาร และไซต์อื่น ๆ)</a></li> </ul> <ul> <li style="font-weight: 400;"><a href="https://docs.microsoft.com/en-us/onedrive/restore-deleted-onedrive">คืนค่าไซต์ OneDrive ถูกลบไปแล้ว</a></li> </ul> <p>สำหรับการดำเนินการจำนวนมากถังรีไซเคิล admins อาจพิจารณาใช้<a href="https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps">Sharepoint ออนไลน์ PNP ได้</a></p> <p><strong>คุณลักษณะการคืนค่าแฟ้ม</strong></p> <p>ถ้าล็อตของแฟ้ม OneDrive หรือ Sharepoint ของคุณได้รับลบ เขียนทับ เสียหาย หรือการติดไวรัส โดยมัลแวร์ คุณสามารถคืนค่ารี OneDrive หรือ Sharepoint ของคุณทั้งหมดไปยังเวลาก่อนหน้า&nbsp;โดยใช้คุณลักษณะการคืนค่าแฟ้มได้</p> <ul> <li><a href="https://support.office.com/en-us/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15">คืนค่าไลบรารี OneDrive</a></li> <li><a href="https://support.office.com/en-us/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US">คืนค่าไลบรารีเอกสาร</a></li> </ul> <p><strong>หมายเหตุ:</strong> ออนไลน์ของ SharePoint เก็บรักษาข้อมูลสำรองของเนื้อหาทั้งหมดสำหรับ 14 วันเพิ่มเติมนอกเหนือจากการลบจริง ถ้าไม่สามารถคืนค่าเนื้อหาผ่านถังรีไซเคิล หรือคืนค่าแฟ้ม ผู้ดูแลสามารถติดต่อฝ่ายสนับสนุนของ Microsoft เพื่อขอคืนค่าใดก็ได้ภายในหน้าต่าง 14 วัน &nbsp;คืนค่าจากการสำรองข้อมูลจะเสร็จสมบูรณ์สำหรับไซต์คอลเลกชันหรือไซต์ย่อย สำหรับแฟ้มเฉพาะ รายการ หรือไลบรารีไม่ได้</p>
