---
title: ทดสอบความเข้ากันได้ของแอป
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
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694860"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="0a69d-102">ทดสอบความเข้ากันได้ของแอป</span><span class="sxs-lookup"><span data-stu-id="0a69d-102">Do app compatibility testing</span></span>

<span data-ttu-id="0a69d-103">ความเข้ากันได้ของแอปพลิเคชันของ Microsoft Edge สูงมาก</span><span class="sxs-lookup"><span data-stu-id="0a69d-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="0a69d-104">ที่จริงแล้ว Microsoft ให้สัญญาว่าจะมีความเข้ากันได้ดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0a69d-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="0a69d-105">หากใช้งานได้กับ Microsoft Edge 45 และเวอร์ชันก่อนหน้า จะใช้งานได้กับ Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="0a69d-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="0a69d-106">หากสามารถใช้งานบน Internet Explorer ได้ ก็จะสามารถใช้งานบน Microsoft Edge ในโหมด Internet Explorer ได้</span><span class="sxs-lookup"><span data-stu-id="0a69d-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="0a69d-107">หากสามารถใช้งานบน Google Chrome ได้ ก็จะสามารถใช้งานบน Microsoft Edge ได้</span><span class="sxs-lookup"><span data-stu-id="0a69d-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="0a69d-108">ถ้าคุณมีแอปพลิเคชันที่เราไม่เป็นไปตามสัญญานี้ เราจะสัญญาว่าจะแก้ไขด้วย[Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="0a69d-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="0a69d-109">แม้ว่าจะสัญญานี้ เราทราบว่าหลายองค์กรต้องตรวจสอบแอปพลิเคชันบางรายการด้วยเหตุผลด้านการปฏิบัติตามกฎข้อบังคับหรือการจัดการความเสี่ยง</span><span class="sxs-lookup"><span data-stu-id="0a69d-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="0a69d-110">แม้ว่าเราคาดหวังว่าสิ่งนี้จะเป็นเรื่องที่ง่ายมาก แต่การจัดระเบียบและอย่างเข้มงวดในการทดสอบแอปก็เป็นเรื่องสําคัญ</span><span class="sxs-lookup"><span data-stu-id="0a69d-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="0a69d-111">มีสองวิธีในการทดสอบความเข้ากันได้ของแอป:</span><span class="sxs-lookup"><span data-stu-id="0a69d-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="0a69d-112">**การทดสอบแล็บ**: แอปพลิเคชันได้รับการทดสอบในสภาพแวดล้อมที่ควบคุมอย่างแน่นหนาด้วยการกําหนดค่าเฉพาะ</span><span class="sxs-lookup"><span data-stu-id="0a69d-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="0a69d-113">**การทดสอบการทดสอบร่อง**: แอปพลิเคชันได้รับการทดสอบโดยผู้ใช้จํานวนจํากัดในสภาพแวดล้อมการงานในแต่ละวันโดยใช้อุปกรณ์ของตนเอง</span><span class="sxs-lookup"><span data-stu-id="0a69d-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="0a69d-114">เลือกวิธีการที่เหมาะสมที่สุดในแต่ละแอป และทดสอบก่อนที่จะเปิดใช้ทั้งองค์กร</span><span class="sxs-lookup"><span data-stu-id="0a69d-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="0a69d-115">เมื่อคุณมั่นใจได้ว่าแอปของคุณเข้ากันได้ คุณก็พร้อมที่จะปรับใช้ Microsoft Edge กับกลุ่มทดลอง</span><span class="sxs-lookup"><span data-stu-id="0a69d-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
