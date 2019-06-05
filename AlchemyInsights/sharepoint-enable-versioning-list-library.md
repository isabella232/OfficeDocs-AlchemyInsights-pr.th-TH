---
title: เปิดใช้งานการกำหนดรุ่นในรายการหรือไลบรารี
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.openlocfilehash: db1f092ecb7698b08e1c77356a08ab110f774bd0
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719815"
---
# <a name="enable-versioning-for-a-sharepoint-list-or-library"></a>เปิดใช้งานการกำหนดรุ่นสำหรับรายการ SharePoint หรือไลบรารี


<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">เมื่อเปิดใช้งานการกำหนดรุ่นในรายการ SharePoint หรือไลบรารีของคุณ คุณสามารถจัดเก็บ ติดตาม และคืนค่าในรายการและแฟ้มในไลบรารีเมื่อใดก็ ตามที่จะเปลี่ยนแปลง กำหนดรุ่น รวมกับการตั้งค่าอื่น ๆ เช่นเช็คเอาท์ ช่วยให้คุณควบคุมเนื้อหาที่มีการลงรายการบัญชีบนไซต์ของคุณ และสามารถกำหนดค่าจริงถ้าคุณเคยมีความต้องการดู หรือคืนค่ารายการหรือแฟ้มรุ่นเก่า มากมาย</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดรุ่นโปรดเยี่ยมชมด้านล่างของบทความ</span></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247">วิธีการกำหนดรุ่นไม่ทำในรายการ SharePoint หรือไลบรารี</a></span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f&amp;ui=en-US&amp;rs=en-US&amp;ad=US">เปิดใช้งาน และกำหนดค่าการกำหนดรุ่นสำหรับรายการหรือไลบรารี</a></span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1">วิธีการดูประวัติรุ่น</a></span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893?ui=en-US&amp;rs=en-US&amp;ad=US">คืนค่ารุ่นก่อนหน้าของแฟ้มใน OneDrive</a></span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2">ดูไฟล์ Office เวอร์ชันก่อนหน้า</a></span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://docs.microsoft.com/en-us/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits">ขีดจำกัดการกำหนดรุ่น</a>&nbsp;</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">หมายเหตุ:</span></u></strong> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><em style="mso-bidi-font-style: normal;">ถ้าคุณเป็นลูกค้า Office 365 รุ่นเดี๋ยวนี้เปิดอยู่ตามค่าเริ่มต้นเมื่อคุณสร้าง OneDrive ใหม่สำหรับไลบรารีของธุรกิจ และดังกล่าวโดยอัตโนมัติจะบันทึกเอกสารรุ่นล่าสุด 500 ซึ่งจะช่วยให้คุณสามารถป้องกันการสูญเสียข้อมูลหรือเอกสารสำคัญ ถ้าคุณมีไลบรารีที่มีอยู่ บน OneDrive ของคุณสำหรับไซต์ธุรกิจ หรือไซต์สำหรับทีมที่ไม่มีการเปิดใช้งานการกำหนดรุ่น คุณสามารถเปิดการกำหนดรุ่นสำหรับอุปกรณ์เหล่านี้เมื่อใดก็ได้</em></span></p>


