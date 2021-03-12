---
title: ชุดแบบสมาพ
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714586"
---
# <a name="replica-set"></a><span data-ttu-id="925bb-102">ชุดแบบสมาพ</span><span class="sxs-lookup"><span data-stu-id="925bb-102">Replica set</span></span>

<span data-ttu-id="925bb-103">AADDS จะเรียกว่าโดเมนที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="925bb-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="925bb-104">จริงๆ แล้วคือตัวควบคุมโดเมนสองตัวที่เรียกใช้และดูแลรักษาโดย Backend</span><span class="sxs-lookup"><span data-stu-id="925bb-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="925bb-105">DCs สองเครื่องจะมีหนึ่ง DC หลักและหนึ่งการซ้อแบบ DC</span><span class="sxs-lookup"><span data-stu-id="925bb-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="925bb-106">การสํารองข้อมูลใน AADDS (โดเมนที่มีการจัดการ) เป็นกระบวนการอัตโนมัติที่จัดการโดยแพลตฟอร์ม Azure</span><span class="sxs-lookup"><span data-stu-id="925bb-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="925bb-107">การสนับสนุน Azure สามารถช่วยคุณคืนค่าจากการสํารองข้อมูลในกรณีที่เกิดปัญหากับโดเมนที่มีการจัดการของคุณ</span><span class="sxs-lookup"><span data-stu-id="925bb-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="925bb-108">คุณสร้างชุดแบบเสมือนแต่ละชุดในเครือข่ายเสมือน</span><span class="sxs-lookup"><span data-stu-id="925bb-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="925bb-109">เครือข่ายเสมือนแต่ละเครือข่ายต้องถูกเพียร์กับเครือข่ายเสมือนอื่นๆ ที่โฮสต์ชุดแบบพรีวิวของโดเมนที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="925bb-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="925bb-110">การกําหนดค่านี้สร้างโทโพโลยีเครือข่ายตาข่ายที่สนับสนุนการกําหนดค่าไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="925bb-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="925bb-111">เครือข่ายเสมือนสามารถรองรับชุดแบบเสมือนหลายชุดได้ ถ้าชุดแบบเสมือนแต่ละชุดอยู่ในเครือข่ายย่อยเสมือนที่ต่างกัน</span><span class="sxs-lookup"><span data-stu-id="925bb-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="925bb-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="925bb-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
