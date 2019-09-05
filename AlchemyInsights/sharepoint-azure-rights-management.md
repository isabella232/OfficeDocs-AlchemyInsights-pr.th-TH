---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b1ec30a55ec0c08b291228ee90771bc56a55a36d
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751763"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="81c65-102">การป้องกันด้วย IRM ไปยังแฟ้ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="81c65-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="81c65-103">ภายใน SharePoint แบบออนไลน์การป้องกัน IRM จะถูกนำไปใช้กับแฟ้มที่ระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="81c65-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="81c65-104">ก่อนที่องค์กรของคุณจะสามารถใช้การป้องกัน IRM คุณต้องตั้งค่าการจัดการสิทธิ์ก่อน</span><span class="sxs-lookup"><span data-stu-id="81c65-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="81c65-105">IRM จะใช้บริการการจัดการสิทธิ์ Azure จากการป้องกันข้อมูล Azure เพื่อเข้ารหัสและกำหนดข้อจำกัดในการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="81c65-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="81c65-106">บางแผน Office ๓๖๕รวมถึงการจัดการสิทธิ์ Azure แต่ไม่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="81c65-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="81c65-107">หากต้องการเรียนรู้เพิ่มเติมโปรดดูที่:</span><span class="sxs-lookup"><span data-stu-id="81c65-107">To learn more, see:</span></span>

- <span data-ttu-id="81c65-108">[โปรแกรมประยุกต์และบริการของ Office สนับสนุนการจัดการสิทธิ์ Azure อย่างไร](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)</span><span class="sxs-lookup"><span data-stu-id="81c65-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="81c65-109">[ตั้งค่าการจัดการสิทธิ์ในข้อมูล (IRM) ในศูนย์กลางการดูแล SharePoint](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)</span><span class="sxs-lookup"><span data-stu-id="81c65-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="81c65-110">การ[เปิดใช้งานไลบรารีเอกสารและรายการของ SharePoint ที่เป็น IRM](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)</span><span class="sxs-lookup"><span data-stu-id="81c65-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="81c65-111">[การจัดการสิทธิ์ในข้อมูลในสำนักงาน](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span><span class="sxs-lookup"><span data-stu-id="81c65-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="81c65-112">[การจัดการสิทธิ์ในข้อมูลในการแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="81c65-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


