---
title: การแก้ไขปัญหาประสิทธิภาพการทํางานของ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733217"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="78cb9-102">การแก้ไขปัญหาประสิทธิภาพการทํางานของ OneDrive</span><span class="sxs-lookup"><span data-stu-id="78cb9-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="78cb9-103">หากคุณประสบปัญหาการซิงค์ที่ช้ากว่าที่คาดไว้ หรือปัญหาประสิทธิภาพการทํางานที่คล้ายกันกับ OneDrive:</span><span class="sxs-lookup"><span data-stu-id="78cb9-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="78cb9-104">ยืนยันว่าไม่มีปัญหาที่ทราบโดยใช้[แดชบอร์ดสถานภาพบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="78cb9-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="78cb9-105">[เปิดใช้งานไฟล์ตามต้องการ](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)เพื่อให้คุณสามารถเข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive โดยไม่ต้องดาวน์โหลดไฟล์ทั้งหมดและใช้พื้นที่จัดเก็บข้อมูลบนอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="78cb9-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="78cb9-106">[ตรวจสอบแนวทางปฏิบัติที่ดีที่สุด](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)สําหรับการวางแผนและประสิทธิภาพของเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="78cb9-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="78cb9-107">[เพิ่มความเร็วในการอัปโหลดและดาวน์โหลด](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)สูงสุดโดยเฉพาะถ้าคุณกําลังซิงค์อุปกรณ์เป็นครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="78cb9-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="78cb9-108">ถ้าคุณกําลังซิงค์ไลบรารีกับสินค้ามากกว่า 100,000 รายการ การซิงค์ OneDrive อาจดูเหมือนติดอยู่เป็นเวลานาน หรือสถานะแสดง การประมวลผล 0KB ของ xMB"</span><span class="sxs-lookup"><span data-stu-id="78cb9-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="78cb9-109">[เรียนรู้เพิ่มเติมเกี่ยวกับการซิงค์ไฟล์มากกว่า 100,000 ไฟล์](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)และ[ขีดจํากัดที่รองรับของ OneDrive ที่มีไฟล์ 300,000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)</span><span class="sxs-lookup"><span data-stu-id="78cb9-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="78cb9-110">เมื่อผู้ใช้เกินขีดจํากัดการใช้งาน SharePoint แบบออนไลน์ throttles ใด ๆ การร้องขอเพิ่มเติมจากบัญชีผู้ใช้นั้นสําหรับรอบระยะเวลาสั้น ๆ</span><span class="sxs-lookup"><span data-stu-id="78cb9-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="78cb9-111">การดําเนินการของผู้ใช้ทั้งหมดจะถูกควบคุมปริมาณในขณะที่เค้นมีผล</span><span class="sxs-lookup"><span data-stu-id="78cb9-111">All user actions are throttled while the throttle is in effect.</span></span>
