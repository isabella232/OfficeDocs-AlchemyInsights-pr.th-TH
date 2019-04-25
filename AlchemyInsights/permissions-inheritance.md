---
title: สืบทอดสิทธิ์
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 5a72a74710a01cf958fa468b80ee67a4034c4383
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372363"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="6ed08-102">วิธีการทำงานของการสืบทอดสิทธิ์ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="6ed08-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="6ed08-103">โดยค่าเริ่มต้น สิทธิ์ใน SharePoint จะถูกสืบทอดจากค่าที่สูงกว่าในลำดับชั้น</span><span class="sxs-lookup"><span data-stu-id="6ed08-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="6ed08-104">ดังนั้น แฟ้มสืบทอดสิทธิ์จากโฟลเดอร์ ซึ่งสืบทอดสิทธิ์จากไลบรารี ที่สืบทอดสิทธิ์จากไซต์ ซึ่งสืบทอดสิทธิ์จากไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="6ed08-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="6ed08-105">สำหรับข้อมูลเกี่ยวกับการเอาสิทธิ์เฉพาะ และคืนค่าการสืบทอด ดู[แก้ไข และจัดการสิทธิ์สำหรับรายการหรือไลบรารี](https://go.microsoft.com/fwlink/?linkid=869946)</span><span class="sxs-lookup"><span data-stu-id="6ed08-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

