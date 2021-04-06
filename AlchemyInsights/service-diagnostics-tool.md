---
title: เครื่องมือการวินิจฉัยบริการของเดสก์ท็อปเสมือนของ Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596045"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="83209-102">เครื่องมือการวินิจฉัยบริการของเดสก์ท็อปเสมือนของ Windows</span><span class="sxs-lookup"><span data-stu-id="83209-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="83209-103">เดสก์ท็อปเสมือนของ Windows (WVD) มีเครื่องมือการวินิจฉัยที่ช่วยให้ผู้ดูแลระบบระบุข้อผิดพลาดผ่านทางส่วนติดต่อเดียว</span><span class="sxs-lookup"><span data-stu-id="83209-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="83209-104">เครื่องมือนี้จะบันทึกข้อมูลที่เกี่ยวข้องกับการวินิจฉัยเมื่อใดก็ตามที่ WVD ถูกใช้งานโดยบุคคลที่ได้รับมอบหมายบทบาท WVD</span><span class="sxs-lookup"><span data-stu-id="83209-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="83209-105">บันทึกแต่ละไฟล์จะมีข้อมูลเกี่ยวกับบทบาท WVD ที่เกี่ยวข้องกับกิจกรรม ข้อความแสดงข้อผิดพลาดที่ปรากฏระหว่างเซสชัน และข้อมูลเกี่ยวกับผู้เช่าและผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="83209-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="83209-106">คุณสามารถกําหนดค่า Azure Log Analytics ให้บันทึกกิจกรรมที่สร้างขึ้นโดยเครื่องมือการวินิจฉัยโดยปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="83209-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="83209-107">สร้างเวิร์กสเปซ Log Analytics ด้วย[พอร์ทัล Azure](https://go.microsoft.com/fwlink/?linkid=2129500)หรือ[Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="83209-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="83209-108">[เชื่อมต่อคอมพิวเตอร์ Windows กับ Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="83209-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="83209-109">รับ ID เวิร์กสเปซและคีย์หลักของเวิร์กสเปซของคุณ</span><span class="sxs-lookup"><span data-stu-id="83209-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="83209-110">ตัวช่วยสร้างการตั้งค่าต้องใช้ข้อมูลนี้เพื่อกําหนดค่าตัวแทนอย่างถูกต้อง และเพื่อให้แน่ใจว่าสามารถสื่อสารกับ Azure Monitor ได้</span><span class="sxs-lookup"><span data-stu-id="83209-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="83209-111">[ส่งข้อมูลการวินิจฉัยไปยังพื้นที่งานของคุณ](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="83209-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="83209-112">คุณสามารถส่งข้อมูลการวินิจฉัยจากผู้เช่า WVD ของคุณไปยัง Log Analytics เพื่อเวิร์กสเปซของคุณ</span><span class="sxs-lookup"><span data-stu-id="83209-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="83209-113">[ระบุและวินิจฉัย](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ปัญหาภายในและภายนอกที่สัมพันธ์กับ WVD</span><span class="sxs-lookup"><span data-stu-id="83209-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="83209-114">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกําหนดค่าเครื่องมือการวินิจฉัยบริการของ WVD ให้ดูใช้การวิเคราะห์ไฟล์บันทึกของฟีเจอร์การวินิจฉัย</span><span class="sxs-lookup"><span data-stu-id="83209-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>