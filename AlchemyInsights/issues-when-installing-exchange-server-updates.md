---
title: ปัญหาเมื่อติดตั้งการอัปเดต Exchange Server
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9421"
ms.openlocfilehash: 04daad34d1097da0039ac63a13f793a550b68414
ms.sourcegitcommit: 13d96a612b67e01c725d5c2a5a0212d824031f6e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696306"
---
# <a name="issues-when-installing-exchange-server-updates"></a><span data-ttu-id="0c753-102">ปัญหาเมื่อติดตั้งการอัปเดต Exchange Server</span><span class="sxs-lookup"><span data-stu-id="0c753-102">Issues when installing Exchange Server updates</span></span>

<span data-ttu-id="0c753-103">ก่อนที่จะติดตั้งการอัปเดต Exchange Server ให้ดูส่วน "หลักปฏิบัติที่ดีที่สุด" ของบทความ [อัปเกรด Exchange เป็นการอัปเดตสะสม](https://docs.microsoft.com/Exchange/plan-and-deploy/install-cumulative-updates)ล่าสุด</span><span class="sxs-lookup"><span data-stu-id="0c753-103">Before installing Exchange Server updates, see the 'Best Practices' section of the article [Upgrade Exchange to the latest Cumulative Update](https://docs.microsoft.com/Exchange/plan-and-deploy/install-cumulative-updates).</span></span> <span data-ttu-id="0c753-104">การติดตั้งการอัปเดตโดยใช้พร้อมท์ CMD ด้วยสิทธิ์ผู้ดูแลจึงจะมีความสําคัญเป็นพิเศษ (เว้นแต่มีการติดตั้งการอัปเดตผ่าน Microsoft Update)</span><span class="sxs-lookup"><span data-stu-id="0c753-104">It is especially important to install updates using the elevated CMD prompt (unless updates are installed through Microsoft Update).</span></span> <span data-ttu-id="0c753-105">ปัญหานี้มีผลกับการอัปเดตสะสมและความปลอดภัย!</span><span class="sxs-lookup"><span data-stu-id="0c753-105">This applies to both Cumulative and Security updates!</span></span>

<span data-ttu-id="0c753-106">ถ้าคุณเห็นข้อผิดพลาดเมื่อติดตั้งการอัปเดตความปลอดภัยหรือหลังจากติดตั้งการอัปเดต ให้ดู [บทความนี้เกี่ยวกับการแก้ไขปัญหาการติดตั้ง](https://aka.ms/exupdatefaq)ล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="0c753-106">If you see errors when installing security updates or after update was installed, see [this article about troubleshooting failed installations](https://aka.ms/exupdatefaq).</span></span>
