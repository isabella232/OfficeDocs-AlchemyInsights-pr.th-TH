---
title: วิธีแก้ไขปัญหาเกี่ยวกับการติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: 447fee84edc65861dc04038cfe6424249e94f843
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823626"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="a3c58-102">วิธีแก้ไขปัญหาเกี่ยวกับการติดตั้ง Office บนเซิร์ฟเวอร์เทอร์มินัล</span><span class="sxs-lookup"><span data-stu-id="a3c58-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="a3c58-103">เมื่อต้องการใช้การเปิดใช้งานคอมพิวเตอร์ที่แชร์ คุณต้องมีการสมัครใช้งานที่มีแอป Microsoft 365 For Enterprise</span><span class="sxs-lookup"><span data-stu-id="a3c58-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="a3c58-104">ตรวจสอบว่าเปิดใช้งานคอมพิวเตอร์ที่แชร์อยู่</span><span class="sxs-lookup"><span data-stu-id="a3c58-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="a3c58-105">ตรวจสอบว่าการเปิดใช้งานสเร็จแล้ว</span><span class="sxs-lookup"><span data-stu-id="a3c58-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="a3c58-106">ตรวจทานข้อความแสดงข้อผิดพลาดเพื่อเปิดใช้งานคอมพิวเตอร์ที่แชร์ ดังนี้</span><span class="sxs-lookup"><span data-stu-id="a3c58-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="a3c58-107">"ผลิตภัณฑ์ที่เราพบในบัญชีผู้ใช้ของคุณไม่สามารถใช้เพื่อเปิดใช้งาน Office ในสถานการณ์คอมพิวเตอร์ที่แชร์ได้"</span><span class="sxs-lookup"><span data-stu-id="a3c58-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="a3c58-108">ข้อผิดพลาดนี้หมายความว่าคุณไม่มีการสมัครใช้งานที่รวมแอป Microsoft 365 For Enterprise</span><span class="sxs-lookup"><span data-stu-id="a3c58-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="a3c58-109">"ผลิตภัณฑ์ที่ไม่มีใบอนุญาต"</span><span class="sxs-lookup"><span data-stu-id="a3c58-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="a3c58-110">ตรวจสอบว่าผู้ใช้ได้รับมอบหมายสิทธิ์การใช้งานแอป Microsoft 365 For Enterprise</span><span class="sxs-lookup"><span data-stu-id="a3c58-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="a3c58-111">ตรวจสอบว่าผู้ใช้ลงชื่อเข้าใช้ด้วยบัญชีผู้ใช้ของตน</span><span class="sxs-lookup"><span data-stu-id="a3c58-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="a3c58-112">ตรวจสอบว่ามีการเชื่อมต่อระหว่างคอมพิวเตอร์ที่แชร์และอินเทอร์เน็ตอยู่</span><span class="sxs-lookup"><span data-stu-id="a3c58-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="a3c58-113">ดูเคล็ดลับการแก้ไขปัญหาอื่นๆ ที่: แก้ไขปัญหา [ด้วยการเปิดใช้งานคอมพิวเตอร์ที่แชร์](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="a3c58-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>