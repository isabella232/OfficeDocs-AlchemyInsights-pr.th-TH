---
title: ซ่อมแซมไฟล์ .pst ก่อนที่จะนำเข้า
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799115"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="b3043-102">ซ่อมแซมไฟล์ .pst ก่อนที่จะนำเข้า</span><span class="sxs-lookup"><span data-stu-id="b3043-102">Repair .pst file before importing</span></span>

<span data-ttu-id="b3043-103">ก่อนที่คุณจะนำเข้าไฟล์ .pst ใน Outlook ให้ตรวจสอบไฟล์ไม่เสียหายโดยการซ่อมแซมไฟล์:</span><span class="sxs-lookup"><span data-stu-id="b3043-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="b3043-104">ออกจาก Outlook</span><span class="sxs-lookup"><span data-stu-id="b3043-104">Exit Outlook.</span></span>

2. <span data-ttu-id="b3043-105">ค้นหาและเรียกใช้ `Scanpst.exe` ในโฟลเดอร์โปรแกรม Office ของคุณ (ไฟล์ C:\Program (x86) \Microsoft Office\root\Office \<Version\> หรือ C:\Program Files\Microsoft Office\root\Office \<Version\> )</span><span class="sxs-lookup"><span data-stu-id="b3043-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="b3043-106">ใน **เครื่องมือซ่อมแซมกล่องจดหมายเข้าของ Microsoft Outlook**ให้คลิก **เรียกดู** เพื่อค้นหาไฟล์ .pst (ตัวอย่างเช่นใน C:\Users \\<ชื่อผู้ใช้ \> \users\ \appdata\local\microsoft\outlook)</span><span class="sxs-lookup"><span data-stu-id="b3043-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="b3043-107">เลือกไฟล์ .pst แล้วคลิก**เปิด**</span><span class="sxs-lookup"><span data-stu-id="b3043-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="b3043-108">คลิก **เริ่ม** เพื่อเริ่มต้นการสแกน</span><span class="sxs-lookup"><span data-stu-id="b3043-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="b3043-109">ถ้าพบข้อผิดพลาดในไฟล์ให้คลิก **ซ่อมแซม**แล้วคลิก **ตกลง** เมื่อการซ่อมแซมเสร็จสมบูรณ์</span><span class="sxs-lookup"><span data-stu-id="b3043-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="b3043-110">ลองนำเข้าไฟล์ .pst ใน Outlook อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="b3043-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="b3043-111">สำหรับข้อมูลเพิ่มเติมให้ดูที่[ซ่อมแซมไฟล์ข้อมูล outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253)และ[แก้ไขปัญหาในการนำเข้าไฟล์ .pst ของ outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="b3043-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
