---
title: แก้ไขปัญหาการลงชื่อเข้าใช้OneDrive
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
ms.openlocfilehash: 7e08dbb4bbc0a1bbaef5e90e4fc21ee87ae90b80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330881"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>แก้ไขปัญหาการลงชื่อเข้าใช้OneDrive

บทความนี้จะอธิบายสถานการณ์สมมติต่อไปนี้:

- แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไคลเอ็นต์ การซิงค์สําหรับ OneDrive
- การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไซต์ OneDrive for Business ของคุณ

**แก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไคลเอ็นต์ การซิงค์สําหรับ OneDrive**

- For steps to resolve error code 0x004de40, see [Error Code 0x8004de40 when signing in to OneDrive](https://docs.microsoft.com/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive).
- ลงชื่อเข้าใช้OneDrive SharePointไซต์ของคุณโดยไปที่ไซต์ แล้วคลิกปุ่ม ซิงค์ ที่ด้านบนของแถบเมนูบนไซต์
- ตรวจสอบให้แน่ใจว่าคุณลงชื่อเข้าใช้ใน OneDrive for Business ไม่ใช่ OneDrive.com ถ้า URL ที่คุณเยี่ยมชมเริ่มต้นด้วย onedrive.live.com ที่ตั้งไม่ใช่สถานที่ตั้งของ OneDrive for business วิธีง่ายๆ ในการให้แน่ใจว่าคุณลงชื่อเข้าใช้ด้วยลิงก์OneDrive for Business: แล้ว https://portal.office.com/onedrive ใช้บัญชีที่โรงเรียนหรือที่โรงเรียนเพื่อเข้าสู่ระบบ
- หากคุณยังคงประสบปัญหา ให้พิจารณา[การรีเซ็ตOneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)
- [ยกเลิกลิงก์OneDrive](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)จาก OneDrive ลงชื่อเข้าใช้ไซต์ OneDrive หรือ SharePoint แล้วคลิกปุ่ม ซิงค์ ที่ด้านบนของแถบเมนูบนไซต์

**การแก้ไขปัญหาเกี่ยวกับการลงชื่อเข้าใช้ไซต์ OneDrive for Business ของคุณ**

- ตรวจสอบให้แน่ใจว่าคุณลงชื่อเข้าใช้ในOneDrive for Business ไม่ใช่ OneDrive.com ถ้า URL ที่คุณเยี่ยมชมเริ่มต้นด้วย onedrive.live.com ของคุณ ไม่ใช่ที่ที่ตั้งของOneDrive for Businessของคุณ วิธีง่ายๆ ในการให้แน่ใจว่าคุณลงชื่อเข้าใช้ด้วยลิงก์OneDrive for Business: แล้ว https://portal.office.com/onedrive ใช้บัญชีที่โรงเรียนหรือที่โรงเรียนเพื่อเข้าสู่ระบบ
- ถ้าคุณถูกเปลี่ยนเส้นทางไปยังหน้าโปรไฟล์Delveของคุณ ผู้ดูแลระบบ Microsoft 365จะต้องให้สิทธิ์แก่ผู้ใช้ในการสร้างOneDrive for Business[ของพวกเขา](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)
- ทดสอบว่าคุณสามารถเยี่ยมชมไซต์ OneDriveโดยใช้การเรียกดู[แบบ InPrivate](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc)ใน Microsoft Edge (หรือฟีเจอร์ที่คล้ายกันในเบราว์เซอร์อื่น)
    - ถ้าการเรียกดูแบบ InPrivate ใช้งานได้[คุณอาจต้องล้างข้อมูล](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4)การเรียกดูMicrosoft Edge (หรือฟีเจอร์ที่คล้ายกันในเบราว์เซอร์อื่น)

**แก้ไขปัญหาการลงชื่อเข้าใช้Officeซิงค์กับOneDrive**

ถ้าคุณได้รับข้อความแสดงข้อผิดพลาดที่Upload **บล็อก****ลงชื่อเข้าใช้เพื่อ** บันทึกไฟล์นี้ หรือ บันทึกสําเนา คุณอาจต้องเอาสําเนาออกและเชื่อมต่อOneDriveใหม่Office [บริการที่เชื่อมต่อของคุณ](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)

**เคล็ดลับการแก้ไขปัญหาอื่นๆ**

ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง สิทธิ์การใช้งาน หรือ[ผู้ใช้ ให้กําหนดสิทธิ์การใช้งานที่ถูกต้องให้กับผู้ใช้ที่ได้รับผลกระทบ](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)

