---
title: นโยบายการป้องกันแอปพลิเคชัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716912"
---
# <a name="application-protection-policy"></a><span data-ttu-id="4d7be-102">นโยบายการป้องกันแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="4d7be-102">Application protection policy</span></span>

<span data-ttu-id="4d7be-103">ถ้าคุณกำลังใช้นโยบายการคุ้มครองแอปพลิเคชันใหม่ (แอป) ให้ดู[ภาพรวมนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/apps/app-protection-policy)</span><span class="sxs-lookup"><span data-stu-id="4d7be-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="4d7be-104">เมื่อต้องการเริ่มต้นใช้งานแอปให้ดู[ที่วิธีการสร้างและกำหนดนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies)</span><span class="sxs-lookup"><span data-stu-id="4d7be-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="4d7be-105">ข้อกำหนดนโยบายการป้องกันแอปพลิเคชัน:</span><span class="sxs-lookup"><span data-stu-id="4d7be-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="4d7be-106">ผู้ใช้มีสิทธิ์การใช้งาน Intune หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="4d7be-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="4d7be-107">ผู้ใช้เป็นสมาชิกของกลุ่มที่มีการกำหนดเป้าหมายโดยนโยบายการป้องกันแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="4d7be-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="4d7be-108">มีเพียงผู้ใช้ขององค์กรเดียวเท่านั้นที่ลงชื่อเข้าใช้แอปที่ได้รับการป้องกันบนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="4d7be-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="4d7be-109">แอปพลิเคชันได้นำไปใช้กับ[INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started)</span><span class="sxs-lookup"><span data-stu-id="4d7be-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="4d7be-110">สำหรับรายการแอปที่สนับสนุน SDK ให้ดูที่ [แอป Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps)ที่ได้รับการป้องกัน</span><span class="sxs-lookup"><span data-stu-id="4d7be-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="4d7be-111">นโยบายจะนำไปใช้หลังจากที่ผู้ใช้ที่ตรงตามข้อกำหนดข้างต้นลงในแอป Intune SDK ที่เปิดใช้งานของ Intune</span><span class="sxs-lookup"><span data-stu-id="4d7be-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="4d7be-112">วิธีที่ง่ายที่สุดในการตรวจสอบว่ามีการนำนโยบายไปใช้หรือไม่โดยต้องการให้ผู้ใช้ตั้งค่า pin ในนโยบาย</span><span class="sxs-lookup"><span data-stu-id="4d7be-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="4d7be-113">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="4d7be-113">For more information, see:</span></span>

[<span data-ttu-id="4d7be-114">คำถามที่ถามบ่อยเกี่ยวกับการแก้ไขปัญหาของแอป/แหม่ม</span><span class="sxs-lookup"><span data-stu-id="4d7be-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="4d7be-115">วิธีตรวจสอบการตั้งค่านโยบายการป้องกันแอปของคุณ</span><span class="sxs-lookup"><span data-stu-id="4d7be-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="4d7be-116">ทำความเข้าใจเกี่ยวกับการกำหนดเวลาการส่งนโยบายการป้องกันแอป</span><span class="sxs-lookup"><span data-stu-id="4d7be-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="4d7be-117">วิธีการตรวจสอบนโยบายการป้องกันแอป</span><span class="sxs-lookup"><span data-stu-id="4d7be-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)