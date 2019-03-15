---
title: อีเมลที่ส่งทอดผ่านทาง Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ea852e315eaf7611d2d405dcfc9e85ab1ccca196
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/14/2019
ms.locfileid: "30574642"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="73172-102">ตั้งค่าอุปกรณ์แบบมัลติฟังก์ชันหรือแอพลิเคชันจะส่งทางอีเมลโดยใช้ Office 365</span><span class="sxs-lookup"><span data-stu-id="73172-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="73172-103">เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกของคุณและขั้นตอนต่าง ๆ ดู[วิธีการตั้งค่าอุปกรณ์แบบมัลติฟังก์ชันหรือแอพลิเคชันจะส่งทางอีเมลโดยใช้ Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4)</span><span class="sxs-lookup"><span data-stu-id="73172-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="73172-104">**หมายเหตุ:** ถ้าคุณมีอุปกรณ์หรือโปรแกรมประยุกต์ที่ใช้เมื่อเร็ว ๆ นี้ หยุดทำงาน โปรดหมายเหตุที่เราเพิ่งได้เริ่มต้น[การปิดใช้งานการเข้ารหัสแบบ 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption)เป็น ที่วางแผนไว้</span><span class="sxs-lookup"><span data-stu-id="73172-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span>  <span data-ttu-id="73172-105">**Windows Server 2003 IIS SMTP จะไม่ทำงาน – จำเป็นต้องมี Windows รุ่นที่ใหม่กว่า**</span><span class="sxs-lookup"><span data-stu-id="73172-105">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span> 

<span data-ttu-id="73172-106">ข้อผิดพลาดทั่วไปที่อาจจะคล้ายกับ: ความล้มเหลวรับรองความถูกต้อง/ข้อผิดพลาด ความล้มเหลวของ TLS/ข้อ ผิดพลาด ข้อผิดพลาดของอัลกอริทึมการเข้ารหัส ไม่ตรงกันอัลกอริทึม หรือการเชื่อมต่อสายหลุดได้</span><span class="sxs-lookup"><span data-stu-id="73172-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span>  <span data-ttu-id="73172-107">โปรดตรวจสอบกับผู้จัดจำหน่ายของโปรแกรมประยุกต์หรืออุปกรณ์เพื่อดู ว่ามีการเข้ารหัสแบบสมัยใหม่ได้รับการสนับสนุน หรือ ถ้าไม่มีการปรับปรุงนี้</span><span class="sxs-lookup"><span data-stu-id="73172-107">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
