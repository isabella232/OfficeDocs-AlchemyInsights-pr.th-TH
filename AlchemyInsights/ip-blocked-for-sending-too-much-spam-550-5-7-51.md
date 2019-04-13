---
title: 1264 IP ที่ถูกบล็อคสำหรับการส่งสแปมมากเกินไป (550 5.7.51)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1264
ms.assetid: f7af4211-9dbe-415c-b0e3-fc20d43c3868
ms.openlocfilehash: d2d92a15a1863f0c4625fd363096fbfd0582a467
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859483"
---
# <a name="access-denied-banned-sender"></a><span data-ttu-id="57663-102">ปฏิเสธการเข้าถึง ห้ามผู้ส่ง</span><span class="sxs-lookup"><span data-stu-id="57663-102">Access denied, banned sender</span></span>

 <span data-ttu-id="57663-103">**ข้อผิดพลาด**: ข้อผิดพลาดของ SMTP จากเซิร์ฟเวอร์ระยะไกลสำหรับการรับสินค้าที่สั่ง โฮสต์:*กับ xxxx*-เหตุผล (*xxx.xxx.xxx.xxx*) com.mail.protection.outlook.com: 550 5.7.511 เข้าถึงถูกปฏิเสธ ห้ามส่ง [*xx.xxx.x.xxx*]</span><span class="sxs-lookup"><span data-stu-id="57663-103">**Error**: SMTP error from remote server for RCPT TO command, host: *xxxx*-com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*) reason: 550 5.7.511 Access denied, banned sender [*xx.xxx.x.xxx*].</span></span> 

<span data-ttu-id="57663-104">ถ้าคุณได้รับข้อผิดพลาดนี้เมื่อส่งอีเมลไปยังผู้รับ Office 365 เอาบัญชีได้รับผลกระทบจากรายชื่อผู้ส่งที่ถูกบล็อกใน[https://sender.office.com](https://sender.office.com)</span><span class="sxs-lookup"><span data-stu-id="57663-104">If you receive this error when sending email to an Office 365 recipient, remove the affected account from the blocked senders list at [https://sender.office.com](https://sender.office.com).</span></span>
