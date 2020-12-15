---
title: Microsoft Edge กำหนดค่าการตั้งค่าความเป็นส่วนตัว
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678862"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="bc6b1-102">Microsoft Edge กำหนดค่าการตั้งค่าความเป็นส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="bc6b1-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="bc6b1-103">ตามค่าเริ่มต้นถ้ามีการปรับใช้ Microsoft Edge บนแพลตฟอร์มที่ไม่ใช่ Windows ข้อมูลการวินิจฉัยและข้อมูลของไซต์จะไม่ถูกส่งไปยัง Microsoft</span><span class="sxs-lookup"><span data-stu-id="bc6b1-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="bc6b1-104">อย่างไรก็ตามถ้า Microsoft Edge ถูกปรับใช้บน Windows 10 ข้อมูลการวินิจฉัยและข้อมูลไซต์จะถูกส่งตามการ [ตั้งค่าข้อมูลการวินิจฉัยของ Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="bc6b1-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="bc6b1-105">เมื่อต้องการกำหนดค่าวิธีที่ Microsoft Edge จัดการการเก็บรวบรวมข้อมูลสำหรับองค์กรของคุณให้ใช้นโยบายกลุ่มต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bc6b1-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="bc6b1-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): นโยบายนี้จะเปิดใช้งานการรายงานการใช้งานและข้อมูลที่เกี่ยวข้องกับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="bc6b1-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="bc6b1-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): นโยบายนี้ส่งข้อมูลไซต์ที่ใช้ในการปรับปรุงบริการของไมโครซอฟท์</span><span class="sxs-lookup"><span data-stu-id="bc6b1-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="bc6b1-108">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[กำหนดค่าการตั้งค่านโยบาย](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)</span><span class="sxs-lookup"><span data-stu-id="bc6b1-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>