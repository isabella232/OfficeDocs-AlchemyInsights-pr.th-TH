---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 4a04134c1e2e6569302756f3b6be213283638a0d
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40046762"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="4e683-102">การป้องกันด้วย IRM ไปยังแฟ้ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="4e683-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="4e683-103">ภายใน SharePoint แบบออนไลน์การป้องกัน IRM จะถูกนำไปใช้กับแฟ้มที่ระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="4e683-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="4e683-104">ก่อนที่องค์กรของคุณจะสามารถใช้การป้องกัน IRM คุณต้องตั้งค่าการจัดการสิทธิ์ก่อน</span><span class="sxs-lookup"><span data-stu-id="4e683-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="4e683-105">IRM จะใช้บริการการจัดการสิทธิ์ Azure จากการป้องกันข้อมูล Azure เพื่อเข้ารหัสและกำหนดข้อจำกัดในการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="4e683-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="4e683-106">บางแผน Office ๓๖๕รวมถึงการจัดการสิทธิ์ Azure แต่ไม่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="4e683-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="4e683-107">หากต้องการเรียนรู้เพิ่มเติมโปรดดูที่:</span><span class="sxs-lookup"><span data-stu-id="4e683-107">To learn more, see:</span></span>

- <span data-ttu-id="4e683-108">[โปรแกรมประยุกต์และบริการของ Office สนับสนุนการจัดการสิทธิ์ Azure อย่างไร](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)</span><span class="sxs-lookup"><span data-stu-id="4e683-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="4e683-109">[ตั้งค่าการจัดการสิทธิ์ในข้อมูล (IRM) ในศูนย์กลางการดูแล SharePoint](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)</span><span class="sxs-lookup"><span data-stu-id="4e683-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="4e683-110">การ[เปิดใช้งานไลบรารีเอกสารและรายการของ SharePoint ที่เป็น IRM](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)</span><span class="sxs-lookup"><span data-stu-id="4e683-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="4e683-111">[การจัดการสิทธิ์ในข้อมูลในสำนักงาน](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span><span class="sxs-lookup"><span data-stu-id="4e683-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="4e683-112">[การจัดการสิทธิ์ในข้อมูลในการแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="4e683-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


