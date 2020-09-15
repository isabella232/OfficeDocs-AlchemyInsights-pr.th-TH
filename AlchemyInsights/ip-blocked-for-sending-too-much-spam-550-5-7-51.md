---
title: ๑๒๖๔ IP ถูกบล็อกสำหรับการส่งสแปมมากเกินไป (๕๕๐ 5.7.51)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1264
ms.assetid: f7af4211-9dbe-415c-b0e3-fc20d43c3868
ms.openlocfilehash: 1a80c9faf463f4bd2e96d9b7f7cc62fdd4b4fad3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695848"
---
# <a name="access-denied-banned-sender"></a><span data-ttu-id="560f9-102">การเข้าถึงถูกปฏิเสธผู้ส่งที่ถูกแบน</span><span class="sxs-lookup"><span data-stu-id="560f9-102">Access denied, banned sender</span></span>

 <span data-ttu-id="560f9-103">**ข้อผิดพลาด**: ข้อผิดพลาด SMTP จากเซิร์ฟเวอร์ระยะไกลสำหรับรับไปยังคำสั่ง host: *xxxx*-com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*) เหตุผล: ๕๕๐ 5.7.511 Access ถูกปฏิเสธผู้ส่งที่ต้องห้าม [*xx.xxx.x.xxx*]</span><span class="sxs-lookup"><span data-stu-id="560f9-103">**Error**: SMTP error from remote server for RCPT TO command, host: *xxxx*-com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*) reason: 550 5.7.511 Access denied, banned sender [*xx.xxx.x.xxx*].</span></span> 

<span data-ttu-id="560f9-104">ถ้าคุณได้รับข้อผิดพลาดนี้เมื่อส่งอีเมลไปยังผู้รับ Microsoft ๓๖๕ให้ลบบัญชีผู้ใช้ที่ได้รับผลกระทบจากรายชื่อผู้ส่งที่ [https://sender.office.com](https://sender.office.com) ถูกบล็อกที่</span><span class="sxs-lookup"><span data-stu-id="560f9-104">If you receive this error when sending email to a Microsoft 365 recipient, remove the affected account from the blocked senders list at [https://sender.office.com](https://sender.office.com).</span></span>
