---
title: การแก้ไขปัญหาสถานะการตรวจสอบสินค้า
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949924"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="c5e3c-102">การแก้ไขปัญหาสถานะการตรวจสอบสินค้า</span><span class="sxs-lookup"><span data-stu-id="c5e3c-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="c5e3c-103">บริการการเตรียมใช้งาน Azure Active Directory (AD) ตรวจสอบสถานภาพของการกำหนดค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="c5e3c-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="c5e3c-104">นอกจากนี้ยังวางแอปที่ไม่แข็งแรงในสถานะการตรวจสอบ **สินค้า**</span><span class="sxs-lookup"><span data-stu-id="c5e3c-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="c5e3c-105">ถ้าส่วนใหญ่หรือทั้งหมดของการโทรที่ทำกับระบบเป้าหมายล้มเหลวอย่างต่อเนื่องแล้วงานการเตรียมใช้งานจะถูกทำเครื่องหมายเป็นในการตรวจสอบ **สินค้า**</span><span class="sxs-lookup"><span data-stu-id="c5e3c-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="c5e3c-106">ตัวอย่างของความล้มเหลวเป็น **ข้อผิดพลาดที่ได้รับเนื่องจากข้อมูลประจำตัวของผู้ดูแลระบบที่ไม่ถูกต้อง**</span><span class="sxs-lookup"><span data-stu-id="c5e3c-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="c5e3c-107">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่การเตรียมใช้งานแอปพลิเคชันในสถานะ](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status)การตรวจสอบสินค้า</span><span class="sxs-lookup"><span data-stu-id="c5e3c-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="c5e3c-108">เมื่อต้องการแก้ไขปัญหาการซิงค์ cloud ให้ดูที่การเตรียมใช้งานปัญหาที่ถูก[กักกัน](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems)</span><span class="sxs-lookup"><span data-stu-id="c5e3c-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
