---
title: การปรับใช้ Add-in Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031425"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>การปรับใช้ Add-in Microsoft 365 Apps

การปรับใช้แบบรวมศูนย์เป็นวิธีที่แนะOffice Add-in กับผู้ใช้และกลุ่มภายในองค์กรของคุณ เมื่อต้องการปรับใช้ Add-in ให้ปฏิบัติตามขั้นตอนด้านล่าง:

**หมายเหตุ:** เมื่อต้องการติดตั้ง Add-in Officeเป็นผู้ใช้แต่ละราย [ให้ดู ดู จัดการ และติดตั้ง Add-in](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)Officeต่างๆ นอกจากนี้ ตรวจสอบให้แน่ใจว่าได้เปิดใช้งานการรับ add-in Office Store แต่ละรายการแล้ว For details, see [Prevent add-in downloads by off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. ตรวจสอบให้แน่ใจว่าสภาพแวดล้อมของคุณตรงตามความต้องการในการปรับใช้ Add-in โดยใช้การปรับใช้แบบรวมศูนย์ โปรดดูรายละเอียดที่[ข้อกฎหมาย](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. ไปที่ **การตั้งค่า**  >  **แอปที่**  >  **รวมรับ** แอปในศูนย์การจัดการ Microsoft 365เพื่อปรับใช้ Add-in 

หมายเหตุ: 

- แอปที่รวมต้องการให้ผู้ดูแลระบบมีสิทธิ์ผู้ดูแลระบบส่วนกลางExchangeสิทธิ์ผู้ดูแลระบบ

- เมื่อปรับใช้ Add-in กับผู้ใช้หลายราย เราขอแนะนนะให้มอบหมายโดยใช้กลุ่มแทนผู้ใช้แต่ละราย For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- การปรับใช้แบบรวมศูนย์ไม่สนับสนุนผู้ใช้ในกลุ่มที่ซ้อนกันหรือกลุ่มที่มีกลุ่มหลัก For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- ตรวจสอบให้แน่ใจว่า บริการการจัดการแอป Microsoft 365 (GUID: '0517ffa1-825d-4aff-9991-3f2336b8a20a') เปิดใช้งานอยู่เพื่อให้ผู้ใช้ลงชื่อเข้าใช้ได้ For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- ถ้าคุณพบปัญหาในการปรับใช้ Add-in โดยใช้แอปที่รวม ให้ลองปรับใช้[โดยใช้ Add-in](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

สำหรับข้อมูลเพิ่มเติม ให้ดู:

[ปรับใช้ Add-in ในศูนย์การจัดการ](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [จัดการ Add-in ในศูนย์การจัดการ](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [ใช้ cmdlet PowerShell ของการปรับใช้แบบรวมศูนย์เพื่อจัดการ Add-in](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [เผยแพร่Office Add-in โดยใช้การปรับใช้แบบรวมศูนย์ผ่านทางศูนย์การจัดการ Microsoft 365](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [การแก้ไขปัญหา: ผู้ใช้ไม่เห็น Add-in](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [การแก้ไขปัญหาข้อผิดพลาดผู้ใช้ที่มีOffice Add-in](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)