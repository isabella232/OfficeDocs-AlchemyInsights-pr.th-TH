---
title: ๑๕๕๔ข้อผิดพลาด Winsock ของ Winsock ๑๐๐๖๑
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698881"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="8ead2-102">ข้อผิดพลาด Winsock ๑๐๐๖๑</span><span class="sxs-lookup"><span data-stu-id="8ead2-102">Winsock error 10061</span></span>

<span data-ttu-id="8ead2-103">รหัสข้อผิดพลาดนี้หมายความว่า Microsoft ไม่สามารถสร้างซ็อกเก็ต TCP (การเชื่อมต่อ) กับโฮสต์เป้าหมายได้</span><span class="sxs-lookup"><span data-stu-id="8ead2-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="8ead2-104">สาเหตุที่น่าจะเป็นที่สุดของข้อผิดพลาดนี้เป็นปัญหาเกี่ยวกับการกำหนดค่าไฟร์วอลล์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="8ead2-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="8ead2-105">เมื่อต้องการแก้ไขปัญหาให้ตรวจสอบการตั้งค่าเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="8ead2-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="8ead2-106">ตรวจสอบการกำหนดค่าไฟร์วอลล์ของคุณด้วยข้อมูลใน [Microsoft ๓๖๕ url และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="8ead2-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="8ead2-107">ถ้ามีข้อผิดพลาดเกิดขึ้นกับ Exchange Online Protection (EOP) คุณควรได้รับการแจ้งให้ทราบก่อนหน้านี้ไปยังการเปลี่ยนแปลงที่[อยู่ IP ของ Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="8ead2-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="8ead2-108">ตรวจสอบว่าผู้ให้บริการอินเทอร์เน็ตของคุณ (ISP) ไม่ได้บล็อกพอร์ต</span><span class="sxs-lookup"><span data-stu-id="8ead2-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="8ead2-109">ตรวจสอบการตั้งค่าสมาร์ทโฮสต์และเซิร์ฟเวอร์เป้าหมายในตัวเชื่อมต่อของคุณ</span><span class="sxs-lookup"><span data-stu-id="8ead2-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="8ead2-110">โปรดสังเกตว่า Microsoft ๓๖๕ไม่ได้บล็อกการเชื่อมต่อที่ *เข้ามา* ในลักษณะนี้</span><span class="sxs-lookup"><span data-stu-id="8ead2-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
