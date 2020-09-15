---
title: แก้ไขปัญหาเกี่ยวกับ Skype for Business บน Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5984"
- "9003195"
ms.openlocfilehash: 794ec70971fc2eff31047f8346284118eb9d6add
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665053"
---
# <a name="troubleshoot-issues-with-skype-for-business-on-mac"></a><span data-ttu-id="875a0-102">แก้ไขปัญหาเกี่ยวกับ Skype for Business บน Mac</span><span class="sxs-lookup"><span data-stu-id="875a0-102">Troubleshoot issues with Skype for Business on Mac</span></span>

<span data-ttu-id="875a0-103">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="875a0-103">For more information, see:</span></span> 

- <span data-ttu-id="875a0-104">ฟีเจอร์บางอย่างเช่นการทำงานของกลุ่มการตอบสนองหรือการสนทนาแบบถาวรอาจไม่พร้อมใช้งานหรือไม่ได้รับการสนับสนุนบนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="875a0-104">Some features, such as Response Group functionality or Persistent Chat, might not be available or supported on the Mac platform.</span></span> <span data-ttu-id="875a0-105">ตรวจสอบว่าฟังก์ชันการทำงานได้รับการสนับสนุนบนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="875a0-105">Verify that the functionality is supported on the Mac platform.</span></span> <span data-ttu-id="875a0-106">สำหรับความพร้อมใช้งานของฟีเจอร์ Mac ให้ดูที่การเปรียบเทียบฟีเจอร์[ไคลเอ็นต์บนอุปกรณ์เคลื่อนที่สำหรับ skype For business](https://technet.microsoft.com/library/Dn951412.aspx)และ[การเปรียบเทียบฟีเจอร์ไคลเอ็นต์เดสก์ท็อปสำหรับ skype for business](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/clients-and-devices/desktop-feature-comparison)</span><span class="sxs-lookup"><span data-stu-id="875a0-106">For Mac feature availability, see [Mobile client feature comparison for Skype for Business](https://technet.microsoft.com/library/Dn951412.aspx) and [Desktop client feature comparison for Skype for Business](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/clients-and-devices/desktop-feature-comparison).</span></span>
- <span data-ttu-id="875a0-107">ถ้าคุณพบปัญหาในการลงชื่อเข้าใช้บนแอป Skype for Business Mac ให้ตรวจสอบให้แน่ใจว่าโทโพโลยีการรับรองความถูกต้องของคุณได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="875a0-107">If you are experiencing a sign-in issue on the Skype for Business Mac app, make sure that your authentication topology is supported.</span></span> <span data-ttu-id="875a0-108">สำหรับข้อมูลโดยละเอียดเกี่ยวกับวิธีการที่ได้รับการสนับสนุนให้ดูที่โท[Skype For business ได้รับการสนับสนุนด้วยการรับรองความถูกต้องที่ทันสมัย](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/modern-authentication/topologies-supported)</span><span class="sxs-lookup"><span data-stu-id="875a0-108">For detailed information about the supported method, see [Skype for Business topologies supported with Modern Authentication](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/modern-authentication/topologies-supported).</span></span>  
- <span data-ttu-id="875a0-109">ถ้าข้อมูลนี้ไม่ตอบคำถามของคุณให้เปิดบัตรสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="875a0-109">If this information doesn't answer your questions, open a Support ticket.</span></span> <span data-ttu-id="875a0-110">รวบรวมข้อมูลให้มากที่สุดเท่าที่จะเป็นไปได้ก่อนที่จะเปิดตั๋ว</span><span class="sxs-lookup"><span data-stu-id="875a0-110">Collect as much information as possible prior to opening the ticket.</span></span> <span data-ttu-id="875a0-111">ตัวอย่างเช่นรวบรวมข้อความบันทึกและข้อผิดพลาดทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="875a0-111">For example, collect all logs and errors messages.</span></span> <span data-ttu-id="875a0-112">เมื่อต้องการรวบรวมไฟล์บันทึกบน Mac ให้ไปที่การกำหนดลักษณะ **แอป SfB**  >  **Preferences**  >  **รวบรวมบันทึก**</span><span class="sxs-lookup"><span data-stu-id="875a0-112">To collect logs on the Mac, go to  **SfB App** > **Preferences** > **Collect logs**.</span></span>  <span data-ttu-id="875a0-113">บันทึกควรมีรายละเอียดให้มากที่สุดเท่าที่จะเป็นไปได้จากการลงชื่อเข้าใช้ไปยังจุดของความล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="875a0-113">The log should include as much detail as possible from sign-in to the point of failure.</span></span>