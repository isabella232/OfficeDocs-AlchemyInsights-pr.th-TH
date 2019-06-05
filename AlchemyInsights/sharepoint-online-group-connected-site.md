---
title: เพิ่มกลุ่มลงในไซต์ SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719500"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>สร้างกลุ่มไซต์ที่เชื่อมโยงใน SharePoint แบบออนไลน์

<p><strong>มีอยู่สองของปัญหาทั่วไปที่พบในขณะที่สร้าง หรือสร้างกลุ่มใหม่ให้เชื่อมต่อไซต์&nbsp;</strong></p>  <p>1.ถ้าคุณได้ลบกลุ่มและไซต์เชื่อมต่ออยู่ และต้องการที่สร้างไซต์อื่นที่ มี URL เดียวกัน คุณจำเป็นต้องการเอาไซต์ก่อนหน้า</p>  <ul>  <li>ดาวน์โหลด<a title="เชลล์จัดการ SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">เชลล์จัดการ SPO</a> -สำหรับข้อมูลเพิ่มเติมในการเริ่มต้นใช้ powershell ดู<a title="เริ่มต้นใช้งานกับเชลล์จัดการออนไลน์ของ SharePoint" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">เริ่มต้นใช้งานกับเชลล์จัดการออนไลน์ของ SharePoint</a> <br /><br /></li>  <li>เอาไซต์ออกจากการใช้ลบไซต์<a title="เอา SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">เอา SPODeletedSite</a> powershell cmdlet</li>  </ul>  <p>ถ้าคุณกำลังสร้างกลุ่มเชื่อมต่อไซต์ และได้รับคำเตือน<strong>'กลุ่มอื่น ด้วยนามแฝงเหมือนกันอยู่แล้วที่มีอยู่'</strong>กลุ่มที่มีอยู่จากการตรวจสอบ<a title="Office 365 จากศูนย์ดูแล" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 จากศูนย์ Admin</a> เมื่อต้องการแก้ไขปัญหา ไม่จำเป็นต้องลบกลุ่มที่มีอยู่ หรือสร้างไซต์ ด้วยนามแฝงแตกต่างกันกำหนด&nbsp;</p>  <p><strong>มีวิธีต่าง ๆ ในการสร้าง และใช้กลุ่มสมัยใหม่กับ SharePoint&nbsp;</strong></p>  <ol>  <li>คุณสามารถเชื่อมต่อไซต์ที่มีอยู่ไปยังกลุ่ม Office 365 สำหรับข้อมูลเพิ่มเติม ดู<a title="กลุ่มที่มี Office 365 ineterface ผู้ใช้ SharePoint โดยใช้การเชื่อมต่อ" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">กลุ่มที่มี Office 365 ineterface ผู้ใช้ SharePoint โดยใช้การเชื่อมต่อ</a></li>  <li>เมื่อต้องการสร้างการเชื่อมโยงไซต์กลุ่ม Office 365 คุณจำเป็นต้องสร้างไซต์สำหรับทีม สำหรับข้อมูลเพิ่มเติม ดู<a title="สร้างไซต์สำหรับทีมใน SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">สร้างไซต์สำหรับทีมใน SharePoint</a></li>  </ol>

