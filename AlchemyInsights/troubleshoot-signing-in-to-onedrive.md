---
title: แก้ไขปัญหาการลงชื่อเข้าใช้ OneDrive
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: a3ad6d9769dab948cb83c04232bb3d8e937a5dc2
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256923"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>แก้ไขปัญหาการลงชื่อเข้าใช้ OneDrive

บทความนี้อธิบายสถานการณ์สมมติต่อไปนี้:

- แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไคลเอ็นต์การซิงค์ OneDrive
- แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไซต์ OneDrive for Business ของคุณ

**แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไคลเอ็นต์การซิงค์ OneDrive**

- ลงชื่อเข้าใช้ไซต์ OneDrive หรือ SharePoint โดยไปที่ไซต์ **แล้ว** คลิกปุ่ม ซิงค์ ที่ด้านบนของแถบเมนูบนไซต์
- ตรวจสอบให้แน่ใจว่าคุณลงชื่อเข้าใช้ OneDrive for Business ไม่ใช่OneDrive.comของคุณ ถ้า URL ที่คุณเยี่ยมชมเริ่มต้นด้วยonedrive.live.comที่ตั้งนั้นไม่ใช่ที่ตั้งของ OneDrive for Business ของคุณ วิธีง่ายๆ เพื่อให้แน่ใจว่าคุณลงชื่อเข้าใช้ OneDrive for Business คือการใช้ลิงก์นี้: https://portal.office.com/onedrive จากนั้นใช้บัญชีที่โรงเรียนหรือที่โรงเรียนเพื่อเข้าสู่ระบบ
- ถ้าคุณยังคงพบปัญหา ให้พิจารณา[รีเซ็ต OneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)
- [ยกเลิกลิงก์บัญชีของคุณจาก OneDrive](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)ลงชื่อเข้าใช้ไซต์ OneDrive หรือ SharePoint แล้วคลิกปุ่ม ซิงค์ที่ด้านบนของแถบเมนูบนไซต์

**แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไซต์ OneDrive for Business ของคุณ**

- ตรวจสอบให้แน่ใจว่าคุณลงชื่อเข้าใช้ OneDrive for Business ไม่ใช่OneDrive.comของคุณ ถ้า URL ที่คุณเยี่ยมชมเริ่มต้นด้วยonedrive.live.com ไม่ใช่ที่ตั้งของ OneDrive for Business ของคุณ วิธีง่ายๆ เพื่อให้แน่ใจว่าคุณลงชื่อเข้าใช้ OneDrive for Business คือการใช้ลิงก์นี้: https://portal.office.com/onedrive จากนั้นใช้บัญชีที่โรงเรียนหรือที่โรงเรียนเพื่อเข้าสู่ระบบ
- ถ้าคุณถูกเปลี่ยนเส้นทางไปยังหน้าโปรไฟล์ Delve ของคุณ ผู้ดูแลระบบ Microsoft 365 จะต้องให้สิทธิ์แก่ผู้ใช้ในการสร้าง[ไซต์ OneDrive for Business ของพวกเขา](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)
- ทดสอบว่าคุณสามารถเยี่ยมชมไซต์ OneDrive โดยใช้การเรียกดู [แบบ InPrivate ใน Microsoft Edge](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) (หรือฟีเจอร์ที่คล้ายกันในเบราว์เซอร์อื่น)
    - ถ้าการเรียกดูแบบ InPrivate ใช้งานได้ คุณอาจต้องล้างข้อมูลการเรียกดู [ใน Microsoft Edge](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4) (หรือฟีเจอร์ที่คล้ายกันในเบราว์เซอร์อื่น)

**แก้ไขปัญหาการลงชื่อเข้าใช้ Office เพื่อซิงค์กับ OneDrive**

ถ้าคุณได้รับข้อความแสดงข้อผิดพลาดที่บอกว่า **อัปโหลด** ถูกบล็อกลงชื่อเข้าใช้เพื่อบันทึกไฟล์นี้ หรือบันทึกสําเนา คุณอาจต้องลบและเชื่อมต่อ [OneDrive ใหม่จากบริการที่เชื่อมต่อ Office](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)ของคุณ

**เคล็ดลับการแก้ไขปัญหาอื่นๆ**

If you're a global, license, or user admin, [assign the correct license to the affected user](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).

