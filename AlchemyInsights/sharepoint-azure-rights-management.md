---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: cc6f93ba8ae3a030f83da5eca2d28dcf38f0f8f7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800915"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="8a6ca-102">การป้องกัน IRM ไปยังไฟล์ SharePoint</span><span class="sxs-lookup"><span data-stu-id="8a6ca-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="8a6ca-103">ภายใน SharePoint Online การป้องกัน IRM จะถูกนำไปใช้กับไฟล์ที่ระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="8a6ca-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="8a6ca-104">ก่อนที่องค์กรของคุณจะสามารถใช้การป้องกัน IRM ได้คุณจะต้องตั้งค่าการจัดการสิทธิ์ก่อน</span><span class="sxs-lookup"><span data-stu-id="8a6ca-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="8a6ca-105">IRM อาศัยบริการการจัดการสิทธิ์ Azure จากการป้องกันข้อมูล Azure เพื่อเข้ารหัสลับและกำหนดข้อจำกัดการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8a6ca-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="8a6ca-106">การสมัครใช้งาน Microsoft ๓๖๕บางรายการรวมถึงการจัดการสิทธิ์ Azure แต่ไม่ใช่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="8a6ca-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="8a6ca-107">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="8a6ca-107">To learn more, see:</span></span>

- <span data-ttu-id="8a6ca-108">[วิธีที่แอปพลิเคชัน Office และบริการสนับสนุนการจัดการสิทธิ์ Azure](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)</span><span class="sxs-lookup"><span data-stu-id="8a6ca-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="8a6ca-109">[ตั้งค่าการจัดการสิทธิ์ในข้อมูล (IRM) ในศูนย์การจัดการ SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center)</span><span class="sxs-lookup"><span data-stu-id="8a6ca-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="8a6ca-110">[IRM เปิดใช้งานไลบรารีเอกสารและรายการ SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)</span><span class="sxs-lookup"><span data-stu-id="8a6ca-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="8a6ca-111">[การจัดการสิทธิ์ในข้อมูลใน Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span><span class="sxs-lookup"><span data-stu-id="8a6ca-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="8a6ca-112">[การจัดการสิทธิ์ในข้อมูลใน Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="8a6ca-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


