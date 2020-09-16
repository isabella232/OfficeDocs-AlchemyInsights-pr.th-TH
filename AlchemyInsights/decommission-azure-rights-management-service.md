---
title: บริการการจัดการสิทธิ์ของ Azure ยกเลิก (RMS)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5070"
- "9002278"
ms.openlocfilehash: 6bacfd0e383c1a7c02b50e60f9626a733ee68cbc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745806"
---
# <a name="decommission-azure-rights-management-service-rms"></a><span data-ttu-id="d9f20-102">บริการการจัดการสิทธิ์ของ Azure ยกเลิก (RMS)</span><span class="sxs-lookup"><span data-stu-id="d9f20-102">Decommission Azure Rights Management Service (RMS)</span></span>

<span data-ttu-id="d9f20-103">ตรวจสอบให้แน่ใจว่าคุณมีสำเนาของคีย์ผู้เช่าการป้องกันข้อมูล Azure ของคุณและโดเมนการประกาศที่เชื่อถือได้ที่เหมาะสม (TPD) ก่อนที่คุณจะปิดใช้งานบริการการจัดการสิทธิ์ของ Azure</span><span class="sxs-lookup"><span data-stu-id="d9f20-103">Make sure that you have a copy of your Azure Information Protection tenant key and a suitable trusted publishing domain (TPD) before you deactivate the Azure Rights Management service.</span></span>

<span data-ttu-id="d9f20-104">สำหรับแหล่งข้อมูลเพิ่มเติมเกี่ยวกับการรื้อถอนและปิดการป้องกันการป้องกันข้อมูล Azure ให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="d9f20-104">For additional resources about decommissioning and deactivating protection for Azure Information Protection, see:</span></span>

- [<span data-ttu-id="d9f20-105">บทช่วยสอน: กำหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่</span><span class="sxs-lookup"><span data-stu-id="d9f20-105">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="d9f20-106">การป้องกันข้อมูล Azure คืออะไร</span><span class="sxs-lookup"><span data-stu-id="d9f20-106">What is Azure Information Protection?</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d9f20-107">เส้นบอกแนววิธีการสำหรับสถานการณ์สมมติทั่วไปที่ใช้การป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="d9f20-107">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
    
- [<span data-ttu-id="d9f20-108">วิธีการโยกย้ายป้ายชื่อการป้องกันข้อมูลของ Azure ไปยังป้ายชื่อความลับแบบครบวงจร</span><span class="sxs-lookup"><span data-stu-id="d9f20-108">How to migrate Azure Information Protection labels to unified sensitivity labels</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)  
    
- [<span data-ttu-id="d9f20-109">การกำหนดราคาการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="d9f20-109">Azure Information Protection pricing</span></span>](https://azure.microsoft.com/pricing/details/information-protection)  
    
- [<span data-ttu-id="d9f20-110">ความต้องการในการป้องกันข้อมูลของ Azure</span><span class="sxs-lookup"><span data-stu-id="d9f20-110">Azure Information Protection requirements</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
    
- [<span data-ttu-id="d9f20-111">วิธีการเปิดใช้งานบริการการป้องกันการจัดการสิทธิ์จากพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="d9f20-111">How to activate the Rights Management protection service from the Azure portal</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-use/activate-azure)