---
title: สถานะโดเมน - ไม่ได้เลือกบริการไว้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389200"
---
# <a name="domain-status---no-services-selected"></a><span data-ttu-id="fbb4c-102">สถานะโดเมน - ไม่ได้เลือกบริการไว้</span><span class="sxs-lookup"><span data-stu-id="fbb4c-102">Domain Status - No services selected</span></span>

<span data-ttu-id="fbb4c-103">ไม่ได้ **เลือกบริการ** ไว้หมายความว่าคุณยังไม่ได้เลือกบริการใดๆ Microsoft 365 เช่น Exchange Online, Skype for Business หรือ Intuned และการจัดการอุปกรณ์เคลื่อนที่Microsoft 365ใช้กับโดเมนแบบปรับแต่งเองของคุณ</span><span class="sxs-lookup"><span data-stu-id="fbb4c-103">**No services selected** means you haven’t selected any Microsoft 365 services such as Exchange Online, Skype for Business or Intune, and Mobile Device Management for Microsoft 365 to use with your custom domain.</span></span> <span data-ttu-id="fbb4c-104">ถ้าคุณใช้งาน Exchange Hybrid (ภายในExchangeองค์กรที่มี Exchange Online) หรือการกรองสแปมภายนอกด้วย Exchange และไม่มีบริการของ Microsoftอื่นๆ คุณสามารถละเว้นข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="fbb4c-104">If you're using Exchange Hybrid (Exchange on-premises with Exchange Online) or external spam filtering with Exchange and no other Microsoft services, you can ignore this message.</span></span> <span data-ttu-id="fbb4c-105">สถานะความสมบูรณ์ของโดเมนจะพร้อมใช้งานเฉพาะโดเมนที่เชื่อมต่อกับบริการโดยตรงเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="fbb4c-105">Domain health status is available only for domains connected directly to the service.</span></span>

<span data-ttu-id="fbb4c-106">เมื่อต้องการเลือกบริการต่างๆ ให้กับโดเมนของคุณ:</span><span class="sxs-lookup"><span data-stu-id="fbb4c-106">To select services for your domain:</span></span>

1. <span data-ttu-id="fbb4c-107">จาก **การตั้งค่า**  >  [**โดเมน**](https://admin.microsoft.com/Adminportal/Home)ของคุณ ให้เลือกกล่องกาเครื่องหมายถัดจากโดเมนที่มีข้อความ **สถานะ ไม่มีบริการ** ที่เลือก</span><span class="sxs-lookup"><span data-stu-id="fbb4c-107">From **Settings** > [**Domains**](https://admin.microsoft.com/Adminportal/Home), check the box next to the domain with the status message **No services selected**.</span></span>
1. <span data-ttu-id="fbb4c-108">เลือก **จัดการ DNS** เพื่อเริ่มตัวช่วยสร้างการตั้งค่าโดเมน</span><span class="sxs-lookup"><span data-stu-id="fbb4c-108">Select **Manage DNS** to start the Domain Setup Wizard.</span></span>
    - <span data-ttu-id="fbb4c-109">ถ้าคุณเลือก **เพิ่มระเบียน DNS ของคุณเอง** ตรวจสอบให้แน่ใจว่าได้เลือกบริการเมื่อได้รับพร้อมท์</span><span class="sxs-lookup"><span data-stu-id="fbb4c-109">If you choose **Add your own DNS records**, be sure to select a service when prompted.</span></span> <span data-ttu-id="fbb4c-110">บริการเพิ่มเติมอาจพร้อมใช้งานภายใต้ **ตัวเลือก** ขั้นสูง</span><span class="sxs-lookup"><span data-stu-id="fbb4c-110">More services could be available under **Advanced Options**.</span></span>
    - <span data-ttu-id="fbb4c-111">ถ้าคุณเลือก ให้ **ไมโครซอฟท์เพิ่มระเบียน DNS ของคุณ** หรือ **ตัวเลือก** เพิ่มเติม ตั้งค่าบริการออนไลน์ของฉันให้ฉัน บริการ  >  ที่พร้อมใช้งานทั้งหมดจะถูกแนะนาและเลือกโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="fbb4c-111">If you choose **Let Microsoft add your DNS records** or **More options** > **Setup my online services for me** all available services are suggested and selected automatically.</span></span>
1. <span data-ttu-id="fbb4c-112">ใช้งานตัวช่วยสร้างต่อไปเพื่อเสร็จสิ้นการตั้งค่า DNS และตัวเลือกบริการของคุณ</span><span class="sxs-lookup"><span data-stu-id="fbb4c-112">Continue through the wizard to complete DNS setup and your service choices.</span></span>
 
<span data-ttu-id="fbb4c-113">For additional help setting up your domain, see [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="fbb4c-113">For additional help setting up your domain, see [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

