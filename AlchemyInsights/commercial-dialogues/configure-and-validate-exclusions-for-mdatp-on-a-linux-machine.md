---
title: กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP บนเครื่อง Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749246"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="e9c4b-102">กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP บนเครื่อง Linux</span><span class="sxs-lookup"><span data-stu-id="e9c4b-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="e9c4b-103">คุณสามารถแยกบางไฟล์ โฟลเดอร์ กระบวนการ และไฟล์ที่เปิดประมวลผลจากการสแกน MDATP ได้</span><span class="sxs-lookup"><span data-stu-id="e9c4b-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="e9c4b-104">การยกเว้นช่วยป้องกันการตรวจหาซอฟต์แวร์และไฟล์ที่ไม่ถูกต้องไม่เฉพาะหรือถูกปรับแต่งให้องค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="e9c4b-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="e9c4b-105">การยกเว้นยังช่วยลดปัญหาด้านประสิทธิภาพการคํานวณที่เกิดจาก MDATP อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="e9c4b-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="e9c4b-106">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[กําหนดค่าและตรวจสอบข้อยกเว้นของ MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="e9c4b-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e9c4b-107">การยกเว้นที่อธิบายในบทความนี้ใช้ไม่ได้กับความสามารถอื่นๆ ของ MDATP for Linux รวมถึงการตรวจหาจุดสิ้นสุดและการตอบกลับ (EDR)</span><span class="sxs-lookup"><span data-stu-id="e9c4b-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="e9c4b-108">ไฟล์ที่คุณแยกออกโดยใช้วิธีที่อธิบายไว้ในบทความนี้ยังคงสามารถทริกเกอร์การแจ้งเตือน EDR และความสามารถในการตรวจจับอื่นๆ ได้</span><span class="sxs-lookup"><span data-stu-id="e9c4b-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
