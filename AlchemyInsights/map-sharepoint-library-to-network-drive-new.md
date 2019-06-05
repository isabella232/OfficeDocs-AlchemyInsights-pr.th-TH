---
title: แผนผังไลบรารี SharePoint ไปยังไดรฟ์เครือข่าย
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 88a1562b81a9f05259e1442f8947f9eee7c973f9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717470"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>แผนผังไลบรารี SharePoint ไปยังไดรฟ์เครือข่าย

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ไลบรารีเป็นไดรฟ์เครือข่ายที่แมปเป็นแบบชั่วคราว และได้รับการสนับสนุน โดย Internet Explorer เท่านั้น ในบางครั้งคุณต้องเปิดไซต์ SharePoint ใน Internet Explorer และเลือก&ldquo;เซ็นอยู่ใน&rdquo;เมื่อต้องการป้องกันไม่ให้เซสชันหมดอายุ แทน<a href="https://support.office.com/en-us/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88">ซิงค์แฟ้ม SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่</a>ซึ่งเป็น<a href="https://support.office.com/en-us/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e">แฟ้มตามความต้องการ</a> เข้าถึงแฟ้มของคุณทั้งหมดใน OneDrive โดยไม่ต้องใช้เนื้อที่เก็บข้อมูลภายในเครื่อง</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">ถ้าคุณเลือกที่จะแมปไดร์ฟแทนการ<a href="https://support.office.com/en-us/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88">ใช้ไคลเอ็นต์การซิงค์ OneDrive ใหม่</a>ให้แน่ใจว่า คุณทำตามขั้นตอน<span style="mso-spacerun: yes;">&nbsp;</span>ในบทความนี้</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u>วิธีการตั้งค่าคอนฟิก และการแก้ไขปัญหาแมปไดรฟ์เครือข่าย</u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US">ตั้งค่าคอนฟิก และการแก้ปัญหาแมปไดรฟ์เครือข่าย</a></span></li> </ul> <p><strong><span style="font-size: 11.0pt; line-height: 107%; font-family: 'Calibri',sans-serif; mso-ascii-theme-font: minor-latin; mso-fareast-font-family: Calibri; mso-fareast-theme-font: minor-latin; mso-hansi-theme-font: minor-latin; mso-bidi-theme-font: minor-latin; mso-ansi-language: EN-US; mso-fareast-language: EN-US; mso-bidi-language: AR-SA;">หมายเหตุ:</span></strong> <span style="font-size: 11.0pt; line-height: 107%; font-family: 'Calibri',sans-serif; mso-ascii-theme-font: minor-latin; mso-fareast-font-family: Calibri; mso-fareast-theme-font: minor-latin; mso-hansi-theme-font: minor-latin; mso-bidi-theme-font: minor-latin; mso-ansi-language: EN-US; mso-fareast-language: EN-US; mso-bidi-language: AR-SA;"><em style="mso-bidi-font-style: normal;">สำหรับ Internet Explorer 10 กับ Windows 8 หรือ Windows 7 ที่ได้รับ&ldquo;ปฏิเสธการเข้าถึง&rdquo;หรือ&ldquo;ไม่สามารถเข้าถึงเส้นทาง&rdquo;เมื่อต้องการแมปไดรฟ์ ติดตั้งโปรแกรมแก้ไขด่วนนี้เพื่อแก้ไขปัญหานี้ ไปที่<a href="https://support.microsoft.com/en-us/help/2846960" target="_blank" rel="noopener">ข้อผิดพลาดเมื่อคุณเปิดไลบรารีเอกสาร SharePoint ใน Windows Explorer หรือแมปไดรฟ์เครือข่ายไปยังไลบรารีหลังจากที่คุณติดตั้ง Internet Explorer 10</a> </em> </span><u></u></p>
