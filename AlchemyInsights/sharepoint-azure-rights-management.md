---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bc0028626c8934e57e5580477b193a70e49d87be
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504230"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="2033c-102">การป้องกัน IRM ไปยังแฟ้มใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="2033c-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="2033c-103">ภายใน SharePoint แบบออนไลน์ การป้องกัน IRM จะนำไปใช้กับแฟ้มในระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="2033c-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="2033c-104">ก่อนที่องค์กรของคุณสามารถใช้การป้องกันด้วย IRM ก่อนอื่นคุณต้องตั้งค่าการจัดการสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="2033c-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="2033c-105">IRM อาศัยบริการ Azure Rights Management จากการป้องกันข้อมูล Azure เพื่อเข้ารหัสลับ และกำหนดข้อจำกัดในการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="2033c-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="2033c-106">บางแผน Office 365 รวม Azure Rights Management แต่ไม่ใช่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="2033c-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="2033c-107">เมื่อต้องการเรียนรู้เพิ่มเติม ดู:</span><span class="sxs-lookup"><span data-stu-id="2033c-107">To learn more, see:</span></span>

- <span data-ttu-id="2033c-108">[โปรแกรมประยุกต์ Office วิธีและบริการสนับสนุนการจัดการสิทธิ์ของ Azure](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)</span><span class="sxs-lookup"><span data-stu-id="2033c-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="2033c-109">[ตั้งค่าสิทธิการจัดการข้อมูล (IRM) ในศูนย์กลางการดูแล SharePoint](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)</span><span class="sxs-lookup"><span data-stu-id="2033c-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="2033c-110">[รายการและไลบรารีเอกสาร SharePoint ที่เปิดใช้งาน IRM](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)</span><span class="sxs-lookup"><span data-stu-id="2033c-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="2033c-111">การ[จัดการสิทธิ์ในข้อมูลใน Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span><span class="sxs-lookup"><span data-stu-id="2033c-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="2033c-112">[ข้อมูลการจัดการสิทธิ์ใน Exchange แบบออนไลน์](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="2033c-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


