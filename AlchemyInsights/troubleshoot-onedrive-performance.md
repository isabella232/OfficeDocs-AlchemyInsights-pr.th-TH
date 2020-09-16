---
title: การแก้ไขปัญหาประสิทธิภาพการทำงานของ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757904"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="252ad-102">การแก้ไขปัญหาประสิทธิภาพการทำงานของ OneDrive</span><span class="sxs-lookup"><span data-stu-id="252ad-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="252ad-103">ถ้าคุณพบว่าการซิงค์ที่คาดว่าจะทำงานช้ากว่าหรือปัญหาประสิทธิภาพการทำงานที่คล้ายคลึงกันกับ OneDrive ให้ทำดังนี้</span><span class="sxs-lookup"><span data-stu-id="252ad-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="252ad-104">ยืนยันว่าไม่มีปัญหาที่ทราบแล้วโดยใช้[แดชบอร์ดความสมบูรณ์ของบริการ](https://portal.office.com/adminportal/home?ref=/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="252ad-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="252ad-105">[เปิดใช้งานไฟล์ตามความต้อง](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) การเพื่อให้คุณสามารถเข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive ได้โดยไม่ต้องดาวน์โหลดทั้งหมดและใช้พื้นที่เก็บข้อมูลบนอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="252ad-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="252ad-106">[ตรวจทานแนวทางปฏิบัติที่ดีที่สุด](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) สำหรับการวางแผนเครือข่ายและประสิทธิภาพการทำงาน</span><span class="sxs-lookup"><span data-stu-id="252ad-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="252ad-107">[เพิ่มความเร็วในการอัปโหลดและดาวน์โหลด](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)โดยเฉพาะอย่างยิ่งถ้าคุณกำลังซิงค์อุปกรณ์เป็นครั้งแรก</span><span class="sxs-lookup"><span data-stu-id="252ad-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="252ad-108">ถ้าคุณกำลังซิงค์ไลบรารีที่มีรายการมากกว่า๑๐๐,๐๐๐รายการการซิงค์ OneDrive อาจดูเหมือนเป็นเวลานานหรือสถานะแสดงการประมวลผล0KB ของ xMB</span><span class="sxs-lookup"><span data-stu-id="252ad-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="252ad-109">[เรียนรู้เพิ่มเติมเกี่ยวกับการซิงค์ไฟล์มากกว่า๑๐๐,๐๐๐](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)และ[การจำกัดจำนวนไฟล์๓๐๐,๐๐๐ที่ได้รับการสนับสนุนของ OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)</span><span class="sxs-lookup"><span data-stu-id="252ad-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="252ad-110">เมื่อผู้ใช้เกินขีดจำกัดการใช้งาน SharePoint Online throttles การร้องขอเพิ่มเติมใดๆจากบัญชีผู้ใช้นั้นเป็นระยะเวลาสั้นๆ</span><span class="sxs-lookup"><span data-stu-id="252ad-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="252ad-111">การกระทำของผู้ใช้ทั้งหมดจะปริมาณขณะที่เค้นอยู่ในลักษณะพิเศษ</span><span class="sxs-lookup"><span data-stu-id="252ad-111">All user actions are throttled while the throttle is in effect.</span></span>
