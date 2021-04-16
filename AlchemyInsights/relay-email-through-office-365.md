---
title: ส่งอีเมลผ่าน Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809674"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="1b0a1-102">ตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="1b0a1-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="1b0a1-103">เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกและขั้นตอนของคุณ ให้ดู[วิธีการตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมลโดยใช้ Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)</span><span class="sxs-lookup"><span data-stu-id="1b0a1-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="1b0a1-104">**หมายเหตุ:** หากคุณมีอุปกรณ์หรือแอปพลิเคชันที่หยุดการใช้งานได้เมื่อเร็วๆ นี้ โปรดทราบว่าเราเพิ่งเริ่มปิดใช้งานรหัส [3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) ตามที่วางแผนไว้</span><span class="sxs-lookup"><span data-stu-id="1b0a1-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="1b0a1-105">เมื่อต้องการดูอุปกรณ์ที่ได้รับผลกระทบ ให้ไปที่รายงาน ไคลเอ็นต์ [การรับรองความถูกต้องของ](https://protection.office.com/mailflow/dashboard)SMTP</span><span class="sxs-lookup"><span data-stu-id="1b0a1-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="1b0a1-106">ข้อผิดพลาดทั่วไปอาจคล้ายกับ: ความล้มเหลว/ข้อผิดพลาดการรับรองความถูกต้อง, ความล้มเหลว/ข้อผิดพลาด TLS, ข้อผิดพลาดอัลกอริทึม Cipher, อัลกอริทึมไม่ตรงกัน หรือการเชื่อมต่อลดลง</span><span class="sxs-lookup"><span data-stu-id="1b0a1-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="1b0a1-107">เมื่อต้องการแก้ไขปัญหา:</span><span class="sxs-lookup"><span data-stu-id="1b0a1-107">To resolve the issue:</span></span>

 - <span data-ttu-id="1b0a1-108">**Windows Server 2003 IIS SMTP จะไม่สามารถใช้งานได้อีกต่อไป โดยต้องมี Windows เวอร์ชันที่ใหม่กว่า**</span><span class="sxs-lookup"><span data-stu-id="1b0a1-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="1b0a1-109">โปรดตรวจสอบกับผู้ออกแอปพลิเคชันหรืออุปกรณ์ของคุณเพื่อดูว่ารหัสรหัสสมัยใหม่ได้รับการสนับสนุนหรือไม่ หรือมีการอัปเดตหรือไม่</span><span class="sxs-lookup"><span data-stu-id="1b0a1-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
