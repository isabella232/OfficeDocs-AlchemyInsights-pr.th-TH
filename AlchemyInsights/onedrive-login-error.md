---
title: ข้อผิดพลาดการเข้าสู่ระบบ OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982548"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="684a3-102">ข้อผิดพลาดการเข้าสู่ระบบ OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="684a3-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="684a3-103">ถ้าคุณได้รับข้อผิดพลาด "AADSTS50011: URL ตอบกลับที่ระบุในการร้องขอไม่ตรงกับการตอบกลับ" เมื่อลงชื่อเข้าใช้แอป OneDrive ให้ตรวจสอบดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="684a3-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="684a3-104">เวอร์ชัน OneDrive ของคุณจำเป็นต้องมีค่าเท่ากับหรือมากกว่าเวอร์ชัน 20.052. XXXX XXXX .</span><span class="sxs-lookup"><span data-stu-id="684a3-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="684a3-105">เมื่อต้องการตรวจสอบเวอร์ชันของคุณให้คลิกที่ไอคอน OneDrive สีน้ำเงินในพื้นที่การแจ้งเตือนเลือก **วิธีใช้ & การตั้งค่า > การตั้งค่า > เกี่ยวกับ**</span><span class="sxs-lookup"><span data-stu-id="684a3-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="684a3-106">เครือข่ายของคุณอาจบล็อกการรับส่งข้อมูลไปยัง **g.live.com** และ **oneclient.sfx.ms**</span><span class="sxs-lookup"><span data-stu-id="684a3-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="684a3-107">ถ้าการรับส่งข้อมูลดังกล่าวถูกบล็อก OneDrive จะไม่สามารถอัปเดตได้เองได้</span><span class="sxs-lookup"><span data-stu-id="684a3-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="684a3-108">ทำงานกับผู้ดูแลระบบเครือข่ายของคุณเพื่อให้แน่ใจว่าคุณสามารถเข้าถึง Url เหล่านั้นได้</span><span class="sxs-lookup"><span data-stu-id="684a3-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="684a3-109">จุดสิ้นสุด[เหล่านี้](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)ควรสามารถเข้าถึงได้สำหรับลูกค้าที่ใช้แผน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="684a3-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="684a3-110">ถ้าคุณต้องการรับเวอร์ชันปัจจุบันของ OneDrive [https://aka.ms/getonedrive](https://aka.ms/getonedrive) ให้เยี่ยมชมด้วยตนเอง</span><span class="sxs-lookup"><span data-stu-id="684a3-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
