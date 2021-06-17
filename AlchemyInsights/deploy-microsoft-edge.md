---
title: ปรับใช้ Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9139"
- "11088"
- "9005291"
- "9006490"
ms.openlocfilehash: 9a51b0cbf6ccb0254ea2ef162530067bbfb5f215
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989772"
---
# <a name="deploy-microsoft-edge"></a><span data-ttu-id="a7474-102">ปรับใช้ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a7474-102">Deploy Microsoft Edge</span></span>

<span data-ttu-id="a7474-103">หลังจากที่คุณได้กําหนดนโยบายของคุณและเสร็จสิ้นการทดสอบความเข้ากันได้ของแอปเริ่มต้นของคุณแล้ว คุณก็พร้อมที่จะปรับใช้กับกลุ่มทดลองของคุณ</span><span class="sxs-lookup"><span data-stu-id="a7474-103">After you've defined your policies and have finished your initial app compatibility testing, you're ready to deploy to your pilot group.</span></span> <span data-ttu-id="a7474-104">การปรับใช้กลุ่มทดลองช่วยให้คุณได้รับข้อเสนอแนะและแก้ไขปัญหาก่อนที่ Microsoft Edge จะเริ่มต้นใช้งานในทั้งองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="a7474-104">Deploying to a pilot group lets you get feedback and fix issues before Microsoft Edge is rolled out to your entire organization.</span></span>

<span data-ttu-id="a7474-105">เครื่องมือต่อไปนี้พร้อมใช้งานในการปรับใช้ Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="a7474-105">The following tools are available to deploy Microsoft Edge:</span></span>

- <span data-ttu-id="a7474-106">[Microsoft Intun1 for Windows](/mem/intune/apps/apps-windows-edge) หรือ [Microsoft Intun1 for macOS](/mem/intune/apps/apps-edge-macos)</span><span class="sxs-lookup"><span data-stu-id="a7474-106">[Microsoft Intune for Windows](/mem/intune/apps/apps-windows-edge) or [Microsoft Intune for macOS](/mem/intune/apps/apps-edge-macos)</span></span>
- [<span data-ttu-id="a7474-107">ตัวจัดการการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="a7474-107">Configuration Manager</span></span>](/DeployEdge/deploy-edge-with-configuration-manager)
- <span data-ttu-id="a7474-108">เครื่องมืออื่นที่ใช้ไฟล์ [MSI ของ Microsoft Edge](https://www.microsoft.com/edge/business/download)</span><span class="sxs-lookup"><span data-stu-id="a7474-108">Another tool using the [MSI file for Microsoft Edge](https://www.microsoft.com/edge/business/download)</span></span>

<span data-ttu-id="a7474-109">**ตรวจสอบการปรับใช้ของคุณ**</span><span class="sxs-lookup"><span data-stu-id="a7474-109">**Validate your deployment**</span></span>

<span data-ttu-id="a7474-110">หลังจากที่คุณปรับใช้การทดสอบทดสอบของคุณแล้ว ให้รวบรวมข้อเสนอแนะจากผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a7474-110">After you deploy your pilot, capture feedback from users.</span></span> <span data-ttu-id="a7474-111">พิจารณาสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="a7474-111">Consider the following:</span></span>
- <span data-ttu-id="a7474-112">**ความเข้ากันได้**: ระบุไซต์ที่เป็นของรายการไซต์องค์กรที่ไม่ได้ระบุระหว่างการค้นพบไซต์</span><span class="sxs-lookup"><span data-stu-id="a7474-112">**Compatibility**: Identify sites that belong on the Enterprise Site List that weren't identified during site discovery.</span></span>
- <span data-ttu-id="a7474-113">**การกําหนดค่า** นโยบาย : ตรวจสอบให้แน่ใจว่าผู้ใช้สามารถใช้ฟีเจอร์หลักและใช้งานในขณะที่ปฏิบัติตามแนวทางด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="a7474-113">**Policy configuration**: Ensure that users can use key features and do their work while following security guidelines.</span></span>
- <span data-ttu-id="a7474-114">**ความง่ายในการใช้งานและฟีเจอร์ใหม่**: ระบุพื้นที่ใดๆ ที่ควรพัฒนาและส่งมอบการฝึกอบรมตามข้อถามของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="a7474-114">**Ease of use and new features**: Identify any areas where training should be developed and delivered based on user questions.</span></span>

<span data-ttu-id="a7474-115">**การปรับใช้ในวงกว้างของ Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="a7474-115">**Broad deployment of Microsoft Edge**</span></span>

<span data-ttu-id="a7474-116">เมื่อคุณได้ปรับใช้การทดสอบทดสอบและอัปเดตแผนการปรับใช้ด้วยการเรียนรู้บทเรียน คุณก็พร้อมที่จะปรับใช้ Microsoft Edge อย่างเต็มรูปแบบกับผู้ใช้ของคุณทุกคนแล้ว</span><span class="sxs-lookup"><span data-stu-id="a7474-116">Once you've deployed the pilot and updated your deployment plan with lessons learnt, you're ready to do a full deployment of Microsoft Edge to all your users.</span></span> <span data-ttu-id="a7474-117">ยินดีด้วย!</span><span class="sxs-lookup"><span data-stu-id="a7474-117">Congratulations!</span></span>

