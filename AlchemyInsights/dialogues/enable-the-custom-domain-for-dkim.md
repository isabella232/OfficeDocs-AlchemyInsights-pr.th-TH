---
title: เปิดใช้งานโดเมนแบบปรับแต่งเองของ DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525158"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="de8c8-102">เปิดใช้งานโดเมนแบบปรับแต่งเองของ DKIM</span><span class="sxs-lookup"><span data-stu-id="de8c8-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="de8c8-103">หลังจากที่คุณสร้างระเบียน CNAME ของคุณแล้ว คุณต้องเปิดใช้งานโดเมน</span><span class="sxs-lookup"><span data-stu-id="de8c8-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="de8c8-104">เมื่อต้องการเปิดใช้งานโดเมน ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="de8c8-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="de8c8-105">นําทางไปยัง[ศูนย์การจัดการ Exchange](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="de8c8-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="de8c8-106">ในบานหน้าต่างด้านซ้าย ให้เลือกการป้องกัน **> dkim**</span><span class="sxs-lookup"><span data-stu-id="de8c8-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="de8c8-107">เลือกโดเมน จากนั้นภายใต้ **เซ็นชื่อข้อความของโดเมนนี้ด้วยลายเซ็น DKIM\*\*\*\*ให้คลิก** เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="de8c8-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="de8c8-108">ทําซ้ําขั้นตอนนี้ในแต่ละโดเมน</span><span class="sxs-lookup"><span data-stu-id="de8c8-108">Repeat this step for each domain.</span></span>

