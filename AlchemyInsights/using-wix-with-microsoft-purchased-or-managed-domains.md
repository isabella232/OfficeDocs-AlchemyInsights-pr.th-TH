---
title: การใช้เว็บไซต์ Wix กับ Microsoft ซื้อหรือโดเมนที่มีการจัดการ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: bef0943c8621043218088abf0deebddf6c19ef50
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664765"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="0c3bb-102">การใช้เว็บไซต์ Wix กับ Microsoft ซื้อหรือโดเมนที่มีการจัดการ</span><span class="sxs-lookup"><span data-stu-id="0c3bb-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="0c3bb-103">สำหรับข้อมูลเกี่ยวกับวิธีการใช้เว็บไซต์ Wix กับโดเมน Microsoft ที่ซื้อหรือที่มีการจัดการให้ดู[อัปเดตระเบียน DNS เพื่อเก็บเว็บไซต์ของคุณไว้กับผู้ให้บริการโฮสต์ปัจจุบันของคุณ](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="0c3bb-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="0c3bb-104">สำหรับรายละเอียดให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="0c3bb-104">For details, see:</span></span> 

- <span data-ttu-id="0c3bb-105">บทความ Wix "การเชื่อมต่อโดเมนกับ Wix โดยใช้วิธีการชี้" ให้คำแนะนำในการเพิ่มระเบียน DNS ตาม outlined ในลิงก์ด้านบนแทนการเปลี่ยนชื่อเซิร์ฟเวอร์เมื่อคุณกำลังใช้ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="0c3bb-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="0c3bb-106">ถ้าคุณเลือกที่จะเปลี่ยนชื่อเซิร์ฟเวอร์เป็น Wix คุณจะต้องสร้างระเบียน DNS ที่ Wix สำหรับ Microsoft</span><span class="sxs-lookup"><span data-stu-id="0c3bb-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="0c3bb-107">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่สร้างระเบียน DNS ที่ Wix สำหรับ Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)</span><span class="sxs-lookup"><span data-stu-id="0c3bb-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="0c3bb-108">ถ้าโดเมนของคุณถูกซื้อจาก Microsoft ชื่อเซิร์ฟเวอร์ไม่สามารถเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="0c3bb-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="0c3bb-109">ถ้าคุณต้องเปลี่ยนชื่อเซิร์ฟเวอร์โดเมนที่ซื้อของ Microsoft จะต้องถูกโอนไปยังผู้ให้บริการโฮสต์อื่นหลังจาก๖๐วัน</span><span class="sxs-lookup"><span data-stu-id="0c3bb-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="0c3bb-110">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การโอนย้ายโดเมนจาก Microsoft ไปยังโฮสต์อื่น](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span><span class="sxs-lookup"><span data-stu-id="0c3bb-110">For more info, see [Transfer a domain from Microsoft to another host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span></span>
