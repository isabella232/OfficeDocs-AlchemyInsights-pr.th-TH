---
title: ส่งต่อ e-mail ผ่านทาง Office ๓๖๕
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ffdaca1ba45a6f273809dbe50a7c40e8610193e1
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666535"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="7159b-102">ตั้งค่าอุปกรณ์มัลติฟังก์ชันหรือแอปพลิเคชันเพื่อส่งเมลโดยใช้ Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="7159b-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="7159b-103">หากต้องการเรียนรู้เกี่ยวกับตัวเลือกและขั้นตอนต่างๆโปรดดู[วิธีตั้งค่าอุปกรณ์มัลติฟังก์ชันหรือแอปพลิเคชันเพื่อส่งเมลโดยใช้ Office ๓๖๕](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4)</span><span class="sxs-lookup"><span data-stu-id="7159b-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="7159b-104">**หมายเหตุ:** หากคุณมีอุปกรณ์หรือแอปพลิเคชันที่หยุดทำงานเมื่อเร็วๆนี้โปรดทราบว่าเราเพิ่งเริ่ม[การปิดใช้การเข้ารหัส 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption)ตามที่วางแผนไว้</span><span class="sxs-lookup"><span data-stu-id="7159b-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="7159b-105">หากต้องการดูอุปกรณ์ที่ได้รับผลกระทบให้ไปที่รายงานการรับรองความถูกต้องของ[ไคลเอนต์ SMTP](https://protection.office.com/mailflow/dashboard)</span><span class="sxs-lookup"><span data-stu-id="7159b-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="7159b-106">ข้อผิดพลาดทั่วไปอาจคล้ายกับ: การตรวจสอบความถูกต้องล้มเหลว/ข้อผิดพลาด TLS ล้มเหลว/ข้อผิดพลาดข้อผิดพลาดของขั้นตอนวิธีการรหัส, อัลกอริทึมไม่ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="7159b-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="7159b-107">หากต้องการแก้ไขปัญหา:</span><span class="sxs-lookup"><span data-stu-id="7159b-107">To resolve the issue:</span></span>
 - <span data-ttu-id="7159b-108">**Windows Server ๒๐๐๓ IIS SMTP จะไม่ทำงานอีกต่อไป–จำเป็นต้องใช้ Windows รุ่นที่ใหม่กว่า**</span><span class="sxs-lookup"><span data-stu-id="7159b-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="7159b-109">กรุณาตรวจสอบกับโปรแกรมประยุกต์หรือผู้จำหน่ายอุปกรณ์ของคุณเพื่อดูว่าการเข้ารหัสที่ทันสมัยได้รับการสนับสนุนหรือไม่มีการปรับปรุง</span><span class="sxs-lookup"><span data-stu-id="7159b-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
