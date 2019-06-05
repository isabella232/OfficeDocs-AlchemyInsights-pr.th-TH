---
title: จำกัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 4d8145ccb60056a4cdaee4b8b9d9e8a4183af571
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715965"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="52c20-102">การป้องกัน IRM ไปยังแฟ้มใน SharePoint</span><span class="sxs-lookup"><span data-stu-id="52c20-102">IRM Protection to SharePoint files</span></span>


<p><span data-ttu-id="52c20-103">ภายใน SharePoint แบบออนไลน์ การป้องกัน IRM จะนำไปใช้กับแฟ้มในระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="52c20-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="52c20-104">ก่อนที่องค์กรของคุณสามารถใช้การป้องกันด้วย IRM ก่อนอื่นคุณต้องตั้งค่าการจัดการสิทธิ์</span><span class="sxs-lookup"><span data-stu-id="52c20-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="52c20-105">IRM อาศัยบริการ Azure Rights Management จากการป้องกันข้อมูล Azure เพื่อเข้ารหัสลับ และกำหนดข้อจำกัดในการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="52c20-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="52c20-106">บางแผน Office 365 รวม Azure Rights Management แต่ไม่ใช่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="52c20-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> <span data-ttu-id="52c20-107">เมื่อต้องการเรียนรู้เพิ่มเติม อ่าน<a href="https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support" data-linktype="external">โปรแกรมประยุกต์ Office วิธีและบริการสนับสนุนการจัดการสิทธิ์ของ Azure</a></span><span class="sxs-lookup"><span data-stu-id="52c20-107">To learn more, read <a href="https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support" data-linktype="external">How Office applications and services support Azure Rights Management</a>.</span></span></p> <ul> <li><span data-ttu-id="52c20-108"><a href="https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-irm-in-sp-admin-center">ตั้งค่าการจัดการสิทธิ์ในข้อมูล (IRM) ในศูนย์กลางการดูแล SharePoint</a></span><span class="sxs-lookup"><span data-stu-id="52c20-108"><a href="https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-irm-in-sp-admin-center">Set up Information Rights Management (IRM) in SharePoint admin center</a></span></span></li> <li><span data-ttu-id="52c20-109"><a href="https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists">เปิดใช้งาน IRM ไลบรารีเอกสารของ SharePoint และรายการ</a></span><span class="sxs-lookup"><span data-stu-id="52c20-109"><a href="https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists">IRM-enable SharePoint document libraries and lists</a></span></span></li> <li><span data-ttu-id="52c20-110"><a href="https://support.office.com/en-US/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c">การจัดการสิทธิ์ในข้อมูลใน Office</a></span><span class="sxs-lookup"><span data-stu-id="52c20-110"><a href="https://support.office.com/en-US/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c">Information Rights Management in Office</a></span></span></li> <li><span data-ttu-id="52c20-111"><a href="https://docs.microsoft.com/en-us/office365/SecurityCompliance/information-rights-management-in-exchange-online">จัดการสิทธิ์ในข้อมูลในการแลกเปลี่ยนแบบออนไลน์</a></span><span class="sxs-lookup"><span data-stu-id="52c20-111"><a href="https://docs.microsoft.com/en-us/office365/SecurityCompliance/information-rights-management-in-exchange-online">Information Rights Management in Exchange Online</a></span></span></li> </ul>


