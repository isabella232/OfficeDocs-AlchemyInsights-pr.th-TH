---
title: แก้ไขปัญหาเกี่ยวกับ Skype สําหรับธุรกิจ บน Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5984"
- "9003195"
ms.openlocfilehash: 5062148ea5bb258cb7d122154d231164310df49d
ms.sourcegitcommit: b9c57ee50d59189784dc57d70a235fe15a9ee6c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555967"
---
# <a name="troubleshoot-issues-with-skype-for-business-on-mac"></a><span data-ttu-id="ca525-102">แก้ไขปัญหาเกี่ยวกับ Skype สําหรับธุรกิจ บน Mac</span><span class="sxs-lookup"><span data-stu-id="ca525-102">Troubleshoot issues with Skype for Business on Mac</span></span>

<span data-ttu-id="ca525-103">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="ca525-103">For more information, see:</span></span> 

- <span data-ttu-id="ca525-104">คุณสมบัติบางอย่าง เช่น ฟังก์ชันการทํางานของกลุ่มการตอบสนอง หรือ การสนทนาแบบถาวร อาจไม่พร้อมใช้งานหรือรองรับบนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="ca525-104">Some features, such as Response Group functionality or Persistent Chat, might not be available or supported on the Mac platform.</span></span> <span data-ttu-id="ca525-105">ตรวจสอบว่าฟังก์ชันการทํางานได้รับการสนับสนุนบนแพลตฟอร์ม Mac</span><span class="sxs-lookup"><span data-stu-id="ca525-105">Verify that the functionality is supported on the Mac platform.</span></span> <span data-ttu-id="ca525-106">สําหรับความพร้อมใช้งานของคุณลักษณะ Mac ดู[การเปรียบเทียบคุณลักษณะไคลเอ็นต์เคลื่อนสําหรับ Skype สําหรับธุรกิจ](https://technet.microsoft.com/library/Dn951412.aspx)และ[เดสก์ท็อปไคลเอ็นต์เปรียบเทียบคุณลักษณะสําหรับ Skype สําหรับธุรกิจ](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/clients-and-devices/desktop-feature-comparison)</span><span class="sxs-lookup"><span data-stu-id="ca525-106">For Mac feature availability, see [Mobile client feature comparison for Skype for Business](https://technet.microsoft.com/library/Dn951412.aspx) and [Desktop client feature comparison for Skype for Business](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/clients-and-devices/desktop-feature-comparison).</span></span>
- <span data-ttu-id="ca525-107">ถ้าคุณประสบปัญหาการเข้าสู่ระบบบน Skype สําหรับโปรแกรมประยุกต์ Mac ธุรกิจ โปรดตรวจสอบให้แน่ใจว่า โทโพโลยีการรับรองความถูกต้องของคุณได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="ca525-107">If you are experiencing a sign-in issue on the Skype for Business Mac app, make sure that your authentication topology is supported.</span></span> <span data-ttu-id="ca525-108">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการได้รับการสนับสนุน ให้ดูที่ การสนับสนุน[Skype for Business โทโพโลจีที่สนับสนุนด้วยการรับรองความถูกต้องแบบสมัยใหม่](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/modern-authentication/topologies-supported)</span><span class="sxs-lookup"><span data-stu-id="ca525-108">For detailed information about the supported method, see [Skype for Business topologies supported with Modern Authentication](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/modern-authentication/topologies-supported).</span></span>  
- <span data-ttu-id="ca525-109">หากข้อมูลนี้ไม่ตอบคําถามของคุณ ให้เปิดตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="ca525-109">If this information doesn't answer your questions, open a Support ticket.</span></span> <span data-ttu-id="ca525-110">รวบรวมข้อมูลให้มากที่สุดก่อนที่จะเปิดตั๋ว</span><span class="sxs-lookup"><span data-stu-id="ca525-110">Collect as much information as possible prior to opening the ticket.</span></span> <span data-ttu-id="ca525-111">ตัวอย่างเช่น รวบรวมแฟ้มบันทึกและข้อความแสดงข้อผิดพลาดทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="ca525-111">For example, collect all logs and errors messages.</span></span> <span data-ttu-id="ca525-112">ในการเก็บรวบรวมบันทึกบน Mac ไปที่การตั้งค่า **แอพ SfB**  >  **Preferences**  >  **เก็บบันทึก**</span><span class="sxs-lookup"><span data-stu-id="ca525-112">To collect logs on the Mac, go to  **SfB App** > **Preferences** > **Collect logs**.</span></span>  <span data-ttu-id="ca525-113">บันทึกควรรวมรายละเอียดมากที่สุดจากการเข้าสู่ระบบไปยังจุดของความล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="ca525-113">The log should include as much detail as possible from sign-in to the point of failure.</span></span>