---
title: การคืนค่า OneDrive ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5298f192-326b-4820-b007-7e1a1c3c2b13
ms.openlocfilehash: f7e99a75fdac420cc2cea0ec10be681bcb2b98ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740926"
---
# <a name="restore-a-deleted-onedrive"></a><span data-ttu-id="5ea5d-102">การคืนค่า OneDrive ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="5ea5d-102">Restore a deleted OneDrive</span></span>

<span data-ttu-id="5ea5d-103">หลังจากที่คุณลบผู้ใช้คุณสามารถเข้าถึง OneDrive ของผู้ใช้ผ่านทางศูนย์การจัดการ Microsoft ๓๖๕สำหรับ30วัน</span><span class="sxs-lookup"><span data-stu-id="5ea5d-103">After you delete a user, you can access the user's OneDrive through the Microsoft 365 admin center for 30 days.</span></span> <span data-ttu-id="5ea5d-104">ผู้ใช้อื่นสามารถเข้าถึงเนื้อหาที่แชร์ใน OneDrive สำหรับระยะเวลาที่คุณตั้งค่าไว้ในศูนย์การจัดการ OneDrive ได้ต่อไป</span><span class="sxs-lookup"><span data-stu-id="5ea5d-104">Other users can continue to access shared content in the OneDrive for the length of time you've set in the OneDrive admin center.</span></span> <span data-ttu-id="5ea5d-105">(เมื่อต้องการเรียนรู้วิธีการตั้งค่านี้ให้ดู [ที่ตั้งค่าการเก็บข้อมูลไฟล์เริ่มต้นสำหรับผู้ใช้ OneDrive ที่ถูกลบ](https://go.microsoft.com/fwlink/?linkid=874267)) หลังจากนั้น OneDrive จะถูกย้ายไปยังถังรีไซเคิลสำหรับ๙๓วันจากนั้นจะถูกลบออก</span><span class="sxs-lookup"><span data-stu-id="5ea5d-105">(To learn how to set this, see [Set the default file retention for deleted OneDrive users](https://go.microsoft.com/fwlink/?linkid=874267).) After that time, the OneDrive is moved to the recycle bin for 93 days, and then it's deleted.</span></span>
  
<span data-ttu-id="5ea5d-106">หลังจาก30วันเริ่มต้นเมื่อผู้ใช้ที่ถูกลบไม่ปรากฏในศูนย์การจัดการ Microsoft ๓๖๕อีกต่อไปคุณสามารถเข้าถึง OneDrive ของผู้ใช้ผ่านทาง PowerShell ได้</span><span class="sxs-lookup"><span data-stu-id="5ea5d-106">After the initial 30 days, when the deleted user no longer appears in the Microsoft 365 admin center, you can access the user's OneDrive through PowerShell.</span></span> <span data-ttu-id="5ea5d-107">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่คืนค่า OneDrive ที่ถูกลบ](https://go.microsoft.com/fwlink/?linkid=874269)</span><span class="sxs-lookup"><span data-stu-id="5ea5d-107">For info, see [Restore a deleted OneDrive](https://go.microsoft.com/fwlink/?linkid=874269).</span></span>
  

