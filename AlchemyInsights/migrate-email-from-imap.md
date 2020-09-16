---
title: โยกย้ายอีเมลจาก IMAP
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "732"
- "1200030"
ms.assetid: 1d51fc10-cb67-4afa-a597-aef8dc90b9f8
ms.openlocfilehash: e59912d98125002cf97a6b4a5201c2c73421c98f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47754862"
---
# <a name="when-you-get-a-not-an-accepted-domain-error"></a><span data-ttu-id="49c95-102">เมื่อคุณได้รับข้อผิดพลาด "ไม่ใช่โดเมนที่ยอมรับ"</span><span class="sxs-lookup"><span data-stu-id="49c95-102">When you get a "Not an accepted domain" error</span></span>

<span data-ttu-id="49c95-103">เมื่อพยายามเพิ่มที่อยู่อีเมลในผู้ใช้หรือกลุ่มหรือในระหว่างการโยกย้ายกล่องจดหมาย Microsoft ๓๖๕คุณอาจได้รับข้อผิดพลาดต่อไปนี้: **คุณไม่สามารถใช้โดเมนได้เนื่องจากไม่ใช่โดเมนที่ยอมรับสำหรับระบบ Exchange ยัง**</span><span class="sxs-lookup"><span data-stu-id="49c95-103">When trying to add an email address on the user or a group or during migration of Microsoft 365 mailboxes, you might be getting the following error: **You can't use the domain because it's not an accepted domain for Exchange System yet.**</span></span>
  
<span data-ttu-id="49c95-104">ในกรณีส่วนใหญ่ข้อผิดพลาดนี้เป็นผลลัพธ์ของชื่อโดเมน *(เช่น contoso.com)*  ไม่ได้ตั้งค่าสำหรับองค์กรของคุณทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="49c95-104">In most cases, this error is a result of the domain name *(such as contoso.com)*  not being fully set up for your organization.</span></span>
  
<span data-ttu-id="49c95-105">โปรดตรวจสอบว่าโดเมนมีการตั้งค่าทั้งหมดโดยทำตามคำแนะนำใน[เพิ่มโดเมนไปยัง Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)</span><span class="sxs-lookup"><span data-stu-id="49c95-105">Please verify that the domain is fully setup by following the instructions in [Add a domain to Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>
  