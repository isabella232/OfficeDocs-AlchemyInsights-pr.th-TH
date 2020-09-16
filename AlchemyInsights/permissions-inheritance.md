---
title: การสืบทอดสิทธิ์
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: f086bd7312772b399146cd81261f147364d64665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741970"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="89662-102">วิธีการทำงานของการสืบทอดสิทธิ์ใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="89662-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="89662-103">ตามค่าเริ่มต้นสิทธิ์ใน SharePoint จะถูกสืบทอดมาจากที่สูงขึ้นในลำดับชั้น</span><span class="sxs-lookup"><span data-stu-id="89662-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="89662-104">ดังนั้นไฟล์จะสืบทอดสิทธิ์จากโฟลเดอร์ซึ่งสืบทอดสิทธิ์จากไลบรารีซึ่งสืบทอดสิทธิ์จากไซต์ซึ่งสืบทอดสิทธิ์จากไซต์คอลเลกชันที่สืบทอดมาจากไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="89662-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="89662-105">สำหรับข้อมูลเกี่ยวกับการเอาสิทธิ์ที่ไม่ซ้ำกันออกและการคืนค่าการสืบทอดให้ดูที่[แก้ไขและจัดการสิทธิ์สำหรับรายการหรือไลบรารี](https://go.microsoft.com/fwlink/?linkid=869946)</span><span class="sxs-lookup"><span data-stu-id="89662-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

