---
title: รีเลย์อีเมลผ่าน Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776505"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="72ef1-102">ตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมล</span><span class="sxs-lookup"><span data-stu-id="72ef1-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="72ef1-103">เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกของคุณและขั้นตอนต่างๆให้ดูที่[วิธีการตั้งค่าอุปกรณ์แบบมัลติฟังก์ชันหรือแอปพลิเคชันเพื่อส่งอีเมลโดยใช้ Microsoft ๓๖๕](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)</span><span class="sxs-lookup"><span data-stu-id="72ef1-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="72ef1-104">**หมายเหตุ:** ถ้าคุณมีอุปกรณ์หรือแอปพลิเคชันที่หยุดทำงานเมื่อเร็วๆนี้โปรดทราบว่าเราได้เริ่ม [การปิดใช้งานการเข้ารหัสการลงจุด](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) ตามแผน</span><span class="sxs-lookup"><span data-stu-id="72ef1-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="72ef1-105">เมื่อต้องการดูอุปกรณ์ที่ได้รับผลกระทบให้ไปที่ [รายงานของไคลเอ็นต์การรับรอง](https://protection.office.com/mailflow/dashboard)ความถูกต้องของ SMTP</span><span class="sxs-lookup"><span data-stu-id="72ef1-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="72ef1-106">ข้อผิดพลาดทั่วไปอาจคล้ายกับ: ความล้มเหลวในการรับรองความถูกต้อง/ข้อผิดพลาด TLS ล้มเหลว/ข้อผิดพลาดของอัลกอริทึมการเข้ารหัสข้อผิดพลาดของอัลกอริทึมไม่ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="72ef1-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="72ef1-107">เมื่อต้องการแก้ไขปัญหาให้ใช้วิธีต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="72ef1-107">To resolve the issue:</span></span>

 - <span data-ttu-id="72ef1-108">**Windows Server ๒๐๐๓ IIS SMTP จะไม่ทำงานอีกต่อไป–จำเป็นต้องใช้ Windows เวอร์ชันที่ใหม่กว่า**</span><span class="sxs-lookup"><span data-stu-id="72ef1-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="72ef1-109">โปรดตรวจสอบกับแอปพลิเคชันหรือผู้จำหน่ายอุปกรณ์ของคุณเพื่อดูว่าการเข้ารหัสที่ทันสมัยได้รับการสนับสนุนหรือไม่หรือถ้ามีการอัปเดต</span><span class="sxs-lookup"><span data-stu-id="72ef1-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
