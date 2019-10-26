---
title: การสืบทอดสิทธิ์
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
ms.openlocfilehash: 6322ca12902be2612f65b6388a650300b257a95e
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36554982"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="9a402-102">วิธีการสืบทอดสิทธิ์ทำงานใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="9a402-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="9a402-103">โดยค่าเริ่มต้นสิทธิ์ใน SharePoint จะได้รับการสืบทอดมาจากสูงขึ้นในลำดับชั้น</span><span class="sxs-lookup"><span data-stu-id="9a402-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="9a402-104">ดังนั้นไฟล์ที่สืบทอดสิทธิ์จากโฟลเดอร์ซึ่งสืบทอดสิทธิ์จากไลบรารีซึ่งสืบทอดสิทธิ์จากเว็บไซต์ซึ่งสืบทอดสิทธิ์จากไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="9a402-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="9a402-105">สำหรับข้อมูลเกี่ยวกับการลบสิทธิ์ที่ไม่ซ้ำกันและการกู้คืนการสืบทอดโปรดดูที่[แก้ไขและจัดการสิทธิ์สำหรับรายการหรือไลบรารี](https://go.microsoft.com/fwlink/?linkid=869946)</span><span class="sxs-lookup"><span data-stu-id="9a402-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

