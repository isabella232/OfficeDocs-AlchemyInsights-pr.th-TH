---
title: นโยบายการป้องกันแอปพลิเคชัน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423958"
---
# <a name="application-protection-policy"></a><span data-ttu-id="0732b-102">นโยบายการป้องกันแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="0732b-102">Application protection policy</span></span>

<span data-ttu-id="0732b-103">หากคุณเพิ่งเริ่มใช้นโยบายการป้องกันแอปพลิเคชัน (APP) โปรดดู[ภาพรวมนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/apps/app-protection-policy)</span><span class="sxs-lookup"><span data-stu-id="0732b-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="0732b-104">เมื่อต้องการเริ่มใช้ APP ให้ดูที่[วิธีสร้างและกําหนดนโยบายการป้องกันแอป](https://docs.microsoft.com/intune/app-protection-policies)</span><span class="sxs-lookup"><span data-stu-id="0732b-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="0732b-105">ข้อกําหนดนโยบายการป้องกันแอปพลิเคชัน:</span><span class="sxs-lookup"><span data-stu-id="0732b-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="0732b-106">ผู้ใช้มีสิทธิ์การใช้งาน Intun หรือ EMS</span><span class="sxs-lookup"><span data-stu-id="0732b-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="0732b-107">ผู้ใช้เป็นสมาชิกของกลุ่มที่กําหนดเป้าหมายตามนโยบายการป้องกันแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="0732b-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="0732b-108">ผู้ใช้ขององค์กรเพียงคนเดียวเท่านั้นที่ลงชื่อเข้าใช้แอปที่มีการป้องกันบนอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="0732b-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="0732b-109">โปรแกรมประยุกต์ได้ดําเนินการ[ใน Intunเย SDK](https://docs.microsoft.com/intune/app-sdk-get-started)</span><span class="sxs-lookup"><span data-stu-id="0732b-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="0732b-110">สําหรับรายการแอปที่สนับสนุน SDK โปรดดู[แอปที่มีการป้องกันของ Microsoft Intun](https://docs.microsoft.com/intune/apps-supported-intune-apps)</span><span class="sxs-lookup"><span data-stu-id="0732b-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="0732b-111">นโยบายจะนําไปใช้หลังจากผู้ใช้ที่มีคุณสมบัติตรงตามข้อกําหนดข้างต้นที่ลงชื่อเข้าใช้แอปที่เปิดใช้งาน Intuner SDK</span><span class="sxs-lookup"><span data-stu-id="0732b-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="0732b-112">วิธีที่ง่ายที่สุดในการตรวจสอบว่ามีการใช้นโยบายหรือไม่</span><span class="sxs-lookup"><span data-stu-id="0732b-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="0732b-113">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="0732b-113">For more information, see:</span></span>

[<span data-ttu-id="0732b-114">คําถามที่พบบ่อยเกี่ยวกับการแก้ไขปัญหาของ APP/MAM</span><span class="sxs-lookup"><span data-stu-id="0732b-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="0732b-115">วิธีตรวจสอบการตั้งค่านโยบายการป้องกันแอป</span><span class="sxs-lookup"><span data-stu-id="0732b-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="0732b-116">ทําความเข้าใจเกี่ยวกับระยะเวลาในการส่งนโยบายการป้องกันแอป</span><span class="sxs-lookup"><span data-stu-id="0732b-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="0732b-117">วิธีตรวจสอบนโยบายการป้องกันแอป</span><span class="sxs-lookup"><span data-stu-id="0732b-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)