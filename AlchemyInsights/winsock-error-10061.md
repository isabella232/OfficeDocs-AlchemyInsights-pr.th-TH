---
title: ข้อผิดพลาด Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530830"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="83001-102">ข้อผิดพลาด Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="83001-102">Winsock error 10061</span></span>

<span data-ttu-id="83001-103">รหัสข้อผิดพลาดนี้หมายความ ว่า Office 365 ไม่สามารถสร้างซ็อกเก็ต TCP (เชื่อมต่อ) กับโฮสต์เป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="83001-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="83001-104">สาเหตุของข้อผิดพลาดนี้น่ามีปัญหากับการกำหนดค่าไฟร์วอลล์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="83001-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="83001-105">เมื่อต้องการแก้ไขปัญหา ตรวจสอบการตั้งค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="83001-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="83001-106">ตรวจสอบการกำหนดค่าไฟร์วอลล์ของคุณกับข้อมูลใน[Office 365 Url และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="83001-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="83001-107">ถ้าข้อผิดพลาดมีการระบุการแลกเปลี่ยนแบบออนไลน์ป้องกัน (EOP), คุณควรได้รับก่อนหน้านี้แจ้งการเปลี่ยนแปลง[ที่อยู่ IP ป้องกันแบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="83001-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="83001-108">ตรวจสอบว่า ผู้ให้บริการอินเทอร์เน็ต (ISP) ของคุณไม่ได้บล็อกพอร์ต</span><span class="sxs-lookup"><span data-stu-id="83001-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="83001-109">ตรวจสอบแบบสมาร์ทโฮสต์และเป้าหมายการตั้งค่าเซิร์ฟเวอร์ในตัวเชื่อมต่อของคุณ</span><span class="sxs-lookup"><span data-stu-id="83001-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="83001-110">หมายเหตุว่า Office 365 ไม่บล็อกการเชื่อมต่อ*ขาเข้า*ในลักษณะนี้</span><span class="sxs-lookup"><span data-stu-id="83001-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
