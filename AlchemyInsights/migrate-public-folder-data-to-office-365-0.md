---
title: โยกย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Microsoft ๓๖๕
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "639"
- "3500007"
ms.assetid: 6e536c7d-ab36-413e-9702-63e51adb3452
ms.openlocfilehash: 778caff63db2c61c07f510309754681c3cab2c56
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674633"
---
# <a name="migrate-public-folder-data-to-microsoft-365"></a><span data-ttu-id="f621b-102">โยกย้ายข้อมูลโฟลเดอร์สาธารณะไปยัง Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="f621b-102">Migrate public folder data to Microsoft 365</span></span>

<span data-ttu-id="f621b-103">ถ้าคุณไม่มีโฟลเดอร์สาธารณะจำนวนมากที่จะนำเข้ามาใน Microsoft ๓๖๕วิธีที่ง่ายที่สุดที่จะนำพวกเขาไปใช้เพื่อคัดลอกข้อมูลลงไป ไฟล์ PST แล้วนำเข้าไฟล์เหล่านั้นลงใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="f621b-103">If you don't have a lot of public folders to bring into Microsoft 365, the easiest way to bring them would be to copy the data into .PST files and then import them into Microsoft 365.</span></span> <span data-ttu-id="f621b-104">สำหรับข้อมูลขนาดเล็กการลากและการวางโฟลเดอร์สาธารณะอย่างง่ายไปยัง a ไฟล์ PST อาจเพียงพอ</span><span class="sxs-lookup"><span data-stu-id="f621b-104">For small amounts of data, a simple drag and drop of public folder into a .PST file can be sufficient.</span></span> <span data-ttu-id="f621b-105">ถ้าคุณมีข้อมูลเพิ่มเติมมากกว่าที่ (สูงสุด 30 GB) เราได้ [บันทึกกระบวนการ](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) ที่คุณสามารถใช้เพื่อส่งออกโฟลเดอร์ไปยังไฟล์ PST</span><span class="sxs-lookup"><span data-stu-id="f621b-105">If you have more data than that (up to 30GB), we have [documented a process](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) that you can use to export folders to PST files.</span></span>
  
<span data-ttu-id="f621b-106">สำหรับองค์กรขนาดใหญ่ที่กำลังย้ายโฟลเดอร์สาธารณะไปยัง Microsoft ๓๖๕เรามีคู่มือที่พร้อมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="f621b-106">For larger organizations who are moving public folders into Microsoft 365, we have guides available:</span></span>
  
- <span data-ttu-id="f621b-107">[โยกย้ายโฟลเดอร์สาธารณะดั้งเดิม](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange ๒๐๑๐)</span><span class="sxs-lookup"><span data-stu-id="f621b-107">[Migrate legacy public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange 2010)</span></span>

- [<span data-ttu-id="f621b-108">โยกย้าย Exchange ๒๐๑๓, Exchange ๒๐๑๖หรือ Exchange ๒๐๑๙โฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="f621b-108">Migrate Exchange 2013, Exchange 2016, or Exchange 2019 public folders</span></span>](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-exchange-online)

<span data-ttu-id="f621b-109">คุณยังมีตัวเลือกในการ[โยกย้ายโฟลเดอร์สาธารณะไปยังกลุ่ม Microsoft ๓๖๕](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-office-365-groups)</span><span class="sxs-lookup"><span data-stu-id="f621b-109">You also have the option to [migrate public folders to Microsoft 365 Groups](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-office-365-groups).</span></span>
  