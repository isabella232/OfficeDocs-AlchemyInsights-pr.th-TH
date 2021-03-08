---
title: เพิ่มโดเมนย่อย
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
ms.openlocfilehash: 08a5d4a51ee8de1a29607bb04ebc05d85faaddaa
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525159"
---
# <a name="add-a-subdomain"></a><span data-ttu-id="3aca5-102">เพิ่มโดเมนย่อย</span><span class="sxs-lookup"><span data-stu-id="3aca5-102">Add a subdomain</span></span>

<span data-ttu-id="3aca5-103">ขั้นตอนในการเพิ่มโดเมนย่อยจะเหมือนกับการเพิ่มโดเมนปกติ</span><span class="sxs-lookup"><span data-stu-id="3aca5-103">The steps for adding a subdomain are the same as adding a regular domain.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="3aca5-104">เมื่อต้องการเพิ่มโดเมนย่อย คุณต้องจัดการการตั้งค่า DNS ของคุณเองที่เว็บไซต์ของบริษัทจดทะเบียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="3aca5-104">To add subdomains, you must manage your own DNS settings at your registrar's website.</span></span> <span data-ttu-id="3aca5-105">ถ้าคุณจะอนุญาตให้ Microsoft จัดการการตั้งค่า DNS ของคุณด้วยระเบียน NS คุณไม่สามารถเพิ่มโดเมนย่อยได้</span><span class="sxs-lookup"><span data-stu-id="3aca5-105">If you're letting Microsoft manage your DNS settings with NS records, you can't add subdomains.</span></span> 

<span data-ttu-id="3aca5-106">เมื่อต้องการเพิ่มโดเมนย่อย ให้ปฏิบัติตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3aca5-106">To add a subdomain, perform the following steps:</span></span>

1. <span data-ttu-id="3aca5-107">ในศูนย์การจัดการ ให้นําทาง **ไปยัง>โดเมน**</span><span class="sxs-lookup"><span data-stu-id="3aca5-107">In the admin center, navigate to **Setup > Domains**.</span></span>
2. <span data-ttu-id="3aca5-108">คลิก **เพิ่ม** โดเมน</span><span class="sxs-lookup"><span data-stu-id="3aca5-108">Click **Add a domain**.</span></span>
3. <span data-ttu-id="3aca5-109">พิมพ์ชื่อของโดเมนย่อย</span><span class="sxs-lookup"><span data-stu-id="3aca5-109">Type the name of the subdomain.</span></span> <span data-ttu-id="3aca5-110">For example, if you own the domain **contoso.com**, your subdomain might be **_london.contoso.com_**.</span><span class="sxs-lookup"><span data-stu-id="3aca5-110">For example, if you own the domain **contoso.com**, your subdomain might be **_london.contoso.com_**.</span></span>
4. <span data-ttu-id="3aca5-111">คลิก **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="3aca5-111">Click **Next**.</span></span>
5. <span data-ttu-id="3aca5-112">หากคุณต้องการตั้งค่าบริการออนไลน์ของโดเมนย่อย ให้ผ่านตัวช่วยสร้าง หรือ</span><span class="sxs-lookup"><span data-stu-id="3aca5-112">If you want to set up online services for the subdomain, continue through the wizard OR</span></span>
6. <span data-ttu-id="3aca5-113">RIf คุณต้องการข้ามการตั้งค่าบริการออนไลน์ของโดเมนย่อย ให้คลิก **บันทึก** แล้วปิดหน้าต่าง</span><span class="sxs-lookup"><span data-stu-id="3aca5-113">RIf you want to skip setting up online services for the subdomain, click **Save** and closethe window.</span></span>

