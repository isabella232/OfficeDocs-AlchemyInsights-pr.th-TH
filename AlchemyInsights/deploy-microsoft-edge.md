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
- "9005291"
ms.openlocfilehash: ad2c42ad77cd4a4606365bc616547846ae3c2c65
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694699"
---
# <a name="deploy-microsoft-edge"></a><span data-ttu-id="3e89c-102">ปรับใช้ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3e89c-102">Deploy Microsoft Edge</span></span>

<span data-ttu-id="3e89c-103">หลังจากที่คุณได้กําหนดนโยบายของคุณและทดสอบความเข้ากันได้ของแอปเริ่มต้นของคุณเสร็จแล้ว คุณก็พร้อมที่จะปรับใช้กับกลุ่มทดลองของคุณ</span><span class="sxs-lookup"><span data-stu-id="3e89c-103">After you've defined your policies and have finished your initial app compatibility testing, you're ready to deploy to your pilot group.</span></span> <span data-ttu-id="3e89c-104">การปรับใช้กลุ่มทดลองช่วยให้คุณได้รับข้อเสนอแนะและแก้ไขปัญหาก่อนที่ Microsoft Edge จะเริ่มต้นใช้งานทั่วทั้งองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="3e89c-104">Deploying to a pilot group lets you get feedback and fix issues before Microsoft Edge is rolled out to your entire organization.</span></span>

<span data-ttu-id="3e89c-105">เครื่องมือต่อไปนี้พร้อมใช้งานเพื่อปรับใช้ Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="3e89c-105">The following tools are available to deploy Microsoft Edge:</span></span>

- <span data-ttu-id="3e89c-106">[Microsoft Intun1 for Windows](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge) หรือ [Microsoft Intun1 for macOS](https://docs.microsoft.com/mem/intune/apps/apps-edge-macos)</span><span class="sxs-lookup"><span data-stu-id="3e89c-106">[Microsoft Intune for Windows](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge) or [Microsoft Intune for macOS](https://docs.microsoft.com/mem/intune/apps/apps-edge-macos)</span></span>
- [<span data-ttu-id="3e89c-107">ตัวจัดการการกําหนดค่า</span><span class="sxs-lookup"><span data-stu-id="3e89c-107">Configuration Manager</span></span>](https://docs.microsoft.com/DeployEdge/deploy-edge-with-configuration-manager)
- <span data-ttu-id="3e89c-108">เครื่องมืออื่นที่ใช้ไฟล์ [MSI ของ Microsoft Edge](https://www.microsoft.com/edge/business/download)</span><span class="sxs-lookup"><span data-stu-id="3e89c-108">Another tool using the [MSI file for Microsoft Edge](https://www.microsoft.com/edge/business/download)</span></span>

<span data-ttu-id="3e89c-109">**ตรวจสอบการปรับใช้งานของคุณ**</span><span class="sxs-lookup"><span data-stu-id="3e89c-109">**Validate your deployment**</span></span>

<span data-ttu-id="3e89c-110">หลังจากที่คุณปรับใช้การทดสอบทดสอบของคุณ แล้ว ให้รวบรวมข้อเสนอแนะจากผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3e89c-110">After you deploy your pilot, capture feedback from users.</span></span> <span data-ttu-id="3e89c-111">พิจารณาสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="3e89c-111">Consider the following:</span></span>
- <span data-ttu-id="3e89c-112">**ความเข้ากันได้**: ระบุไซต์ที่เป็นของรายการไซต์องค์กรที่ระบุตัวตนไม่ได้ระหว่างการค้นพบไซต์</span><span class="sxs-lookup"><span data-stu-id="3e89c-112">**Compatibility**: Identify sites that belong on the Enterprise Site List that weren't identified during site discovery.</span></span>
- <span data-ttu-id="3e89c-113">**การกําหนด** ค่านโยบาย : ตรวจสอบให้แน่ใจว่าผู้ใช้สามารถใช้ฟีเจอร์หลักและใช้งานพร้อมกับปฏิบัติตามแนวทางด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="3e89c-113">**Policy configuration**: Ensure that users can use key features and do their work while following security guidelines.</span></span>
- <span data-ttu-id="3e89c-114">**ความง่ายในการใช้งานและฟีเจอร์** ใหม่ : ระบุพื้นที่ใดๆ ที่ควรพัฒนาและส่งมอบการฝึกอบรมโดยยึดตามข้อถามของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="3e89c-114">**Ease of use and new features**: Identify any areas where training should be developed and delivered based on user questions.</span></span>

<span data-ttu-id="3e89c-115">**การปรับใช้ Microsoft Edge อย่างกว้างๆ**</span><span class="sxs-lookup"><span data-stu-id="3e89c-115">**Broad deployment of Microsoft Edge**</span></span>

<span data-ttu-id="3e89c-116">เมื่อคุณปรับใช้การทดสอบทดสอบและอัปเดตแผนการปรับใช้ด้วยการเรียนรู้บทเรียน คุณก็พร้อมที่จะปรับใช้ Microsoft Edge อย่างเต็มรูปแบบกับผู้ใช้ของคุณทุกคน</span><span class="sxs-lookup"><span data-stu-id="3e89c-116">Once you've deployed the pilot and updated your deployment plan with lessons learnt, you're ready to do a full deployment of Microsoft Edge to all your users.</span></span> <span data-ttu-id="3e89c-117">ขอแสดงความยินดี!</span><span class="sxs-lookup"><span data-stu-id="3e89c-117">Congratulations!</span></span>

