---
title: ใช้การบันทึกการใช้งานสำหรับการจัดการสิทธิ์ Azure
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
- "5506"
- "9002281"
ms.openlocfilehash: f1483e177ec6fcdd39d0aae481d3b329b11577d4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796811"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="895fa-102">ใช้การบันทึกการใช้งานสำหรับการจัดการสิทธิ์ Azure</span><span class="sxs-lookup"><span data-stu-id="895fa-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="895fa-103">ตามค่าเริ่มต้นการบันทึกการใช้งานการป้องกันจะถูกเปิดใช้งานสำหรับลูกค้าทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="895fa-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="895fa-104">บันทึกจะถูกเขียนเป็นชุดของ blobs ในที่เก็บข้อมูล Azure สำหรับผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="895fa-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="895fa-105">หลังจากการดำเนินการป้องกันอาจใช้เวลาถึง15นาทีเพื่อให้การบันทึกมากที่สุดปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="895fa-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="895fa-106">คุณสามารถใช้บันทึกการใช้งานการป้องกันเพื่อ:</span><span class="sxs-lookup"><span data-stu-id="895fa-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="895fa-107">วิเคราะห์ข้อมูลเชิงลึกของธุรกิจ</span><span class="sxs-lookup"><span data-stu-id="895fa-107">Analyze business insights</span></span>

- <span data-ttu-id="895fa-108">ตรวจสอบสำหรับการใช้งานที่ไม่เหมาะสม</span><span class="sxs-lookup"><span data-stu-id="895fa-108">Monitor for abuse</span></span>

- <span data-ttu-id="895fa-109">ดำเนินการวิเคราะห์ทางนิติวิทยาศาสตร์</span><span class="sxs-lookup"><span data-stu-id="895fa-109">Perform forensic analysis</span></span>

<span data-ttu-id="895fa-110">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การบันทึกและการวิเคราะห์การใช้งานการป้องกันจากการป้องกันข้อมูล Azure](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)</span><span class="sxs-lookup"><span data-stu-id="895fa-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="895fa-111">สำหรับข้อมูลเกี่ยวกับการบันทึกการใช้งานไคลเอ็นต์ให้ดูที่[คู่มือสำหรับผู้ดูแลระบบ: ไฟล์ไคลเอ็นต์การป้องกันข้อมูล Azure และการบันทึกการใช้งานไคลเอ็นต์](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)</span><span class="sxs-lookup"><span data-stu-id="895fa-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="895fa-112">สำหรับข้อมูลเพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="895fa-112">For additional information, see:</span></span>

- <span data-ttu-id="895fa-113">[ความต้องการในการป้องกันข้อมูลของ Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span><span class="sxs-lookup"><span data-stu-id="895fa-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="895fa-114">[บทช่วยสอน: กำหนดค่าการตั้งค่านโยบายการป้องกันข้อมูล Azure และสร้างป้ายชื่อใหม่](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)</span><span class="sxs-lookup"><span data-stu-id="895fa-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>