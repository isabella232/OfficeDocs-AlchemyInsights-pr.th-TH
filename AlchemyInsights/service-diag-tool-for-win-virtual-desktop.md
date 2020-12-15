---
title: เครื่องมือการวินิจฉัยบริการสำหรับ Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680234"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="e25a7-102">เครื่องมือการวินิจฉัยบริการสำหรับ Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="e25a7-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="e25a7-103">Windows Virtual Desktop (WVD) มีเครื่องมือการวินิจฉัยที่ช่วยให้ผู้ดูแลระบบสามารถระบุข้อผิดพลาดผ่านทางส่วนติดต่อเดียว</span><span class="sxs-lookup"><span data-stu-id="e25a7-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="e25a7-104">เครื่องมือนี้จะบันทึกข้อมูลที่เกี่ยวข้องกับการวินิจฉัยเมื่อใดก็ตามที่ WVD ถูกใช้งานโดยผู้ที่ได้รับมอบหมายบทบาท WVD</span><span class="sxs-lookup"><span data-stu-id="e25a7-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="e25a7-105">แต่ละแฟ้มบันทึกจะมีข้อมูลเกี่ยวกับบทบาท WVD ที่เกี่ยวข้องกับกิจกรรมข้อความแสดงข้อผิดพลาดที่ปรากฏขึ้นในระหว่างเซสชันและข้อมูลเกี่ยวกับผู้เช่าและผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="e25a7-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="e25a7-106">การวิเคราะห์บันทึกของ Azure สามารถกำหนดค่าให้จับภาพบันทึกกิจกรรมที่สร้างขึ้นโดยเครื่องมือการวินิจฉัยได้</span><span class="sxs-lookup"><span data-stu-id="e25a7-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="e25a7-107">โดยมีวิธีการดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e25a7-107">Here's how:</span></span>

1. <span data-ttu-id="e25a7-108">สร้างเวิร์กสเปซการวิเคราะห์บันทึกที่มี[พอร์ทัล azure](https://go.microsoft.com/fwlink/?linkid=2129500)หรือ[azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="e25a7-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="e25a7-109">[เชื่อมต่อคอมพิวเตอร์ที่มี Windows กับหน้าจอ Azure](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="e25a7-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="e25a7-110">รับ ID ของเวิร์กสเปซและคีย์หลักของพื้นที่ทำงานของคุณ</span><span class="sxs-lookup"><span data-stu-id="e25a7-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="e25a7-111">ตัวช่วยสร้างการตั้งค่าต้องการข้อมูลนี้เพื่อกำหนดค่าตัวแทนอย่างถูกต้องและตรวจสอบให้แน่ใจว่าสามารถสื่อสารกับหน้าจอ Azure ได้อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="e25a7-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="e25a7-112">[ผลักดันข้อมูลการวินิจฉัยไปยังพื้นที่ทำงานของคุณ](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="e25a7-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="e25a7-113">คุณสามารถผลักดันการวินิจฉัยข้อมูลจากผู้เช่า WVD ของคุณไปยังการวิเคราะห์บันทึกสำหรับพื้นที่ทำงานของคุณ</span><span class="sxs-lookup"><span data-stu-id="e25a7-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="e25a7-114">[ระบุและวินิจฉัยปัญหา](https://go.microsoft.com/fwlink/?linkid=2128338) ที่เกี่ยวข้องกับ WVD ภายในหรือภายนอก</span><span class="sxs-lookup"><span data-stu-id="e25a7-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="e25a7-115">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการกำหนดค่าเครื่องมือการวินิจฉัยของบริการสำหรับ WVD ให้ดูที่[ใช้การวิเคราะห์บันทึกสำหรับฟีเจอร์การวินิจฉัย](https://go.microsoft.com/fwlink/?linkid=2128084)</span><span class="sxs-lookup"><span data-stu-id="e25a7-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
