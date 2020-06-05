---
title: การสืบทอดสิทธิ์
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 791085593433dcad9b800fdea8c7ea4a878604e7
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581070"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="e1d6a-102">วิธีการสืบทอดสิทธิ์ทํางานใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="e1d6a-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="e1d6a-103">โดยค่าเริ่มต้น สิทธิ์ใน SharePoint จะถูกสืบทอดจากลําดับชั้นที่สูงกว่า</span><span class="sxs-lookup"><span data-stu-id="e1d6a-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="e1d6a-104">ดังนั้นแฟ้มสืบทอดสิทธิ์จากโฟลเดอร์ ซึ่งสืบทอดสิทธิ์จากไลบรารี ซึ่งสืบทอดสิทธิ์จากไซต์ ซึ่งสืบทอดสิทธิ์จากไซต์คอลเลกชัน</span><span class="sxs-lookup"><span data-stu-id="e1d6a-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="e1d6a-105">สําหรับข้อมูลเกี่ยวกับการเอาสิทธิ์เฉพาะออกและการคืนค่าการสืบทอด ให้ดูที่[แก้ไขและจัดการสิทธิ์สําหรับรายการหรือไลบรารี](https://go.microsoft.com/fwlink/?linkid=869946)</span><span class="sxs-lookup"><span data-stu-id="e1d6a-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

