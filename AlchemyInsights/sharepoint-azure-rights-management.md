---
title: จํากัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 8b5f22269cab0ed0984bcb33703b49e943ef2446
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642271"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="103f1-102">การป้องกัน IRM ไปยังแฟ้ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="103f1-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="103f1-103">ภายใน SharePoint Online การป้องกัน IRM จะถูกนําไปใช้กับแฟ้มที่ระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="103f1-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="103f1-104">ก่อนที่องค์กรของคุณจะใช้การป้องกันด้วย IRM คุณต้องตั้งค่าการจัดการสิทธิ์ก่อน</span><span class="sxs-lookup"><span data-stu-id="103f1-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="103f1-105">IRM อาศัยบริการการจัดการสิทธิ์ Azure จาก Azure การป้องกันข้อมูลเพื่อเข้ารหัสลับ และกําหนดข้อจํากัดการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="103f1-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="103f1-106">การสมัครใช้งาน Microsoft 365 บางรายการมีการจัดการสิทธิ์ Azure แต่ไม่ใช่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="103f1-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="103f1-107">หากต้องการเรียนรู้เพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="103f1-107">To learn more, see:</span></span>

- <span data-ttu-id="103f1-108">[วิธีที่โปรแกรมประยุกต์และบริการ Office สนับสนุนการจัดการสิทธิ์ Azure](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)</span><span class="sxs-lookup"><span data-stu-id="103f1-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="103f1-109">[ตั้งค่าการจัดการสิทธิ์ในข้อมูล (IRM) ใน ศูนย์การจัดการ SharePoint](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)</span><span class="sxs-lookup"><span data-stu-id="103f1-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="103f1-110">[ไลบรารีเอกสารและรายการ SharePoint ที่เปิดใช้งาน IRM](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)</span><span class="sxs-lookup"><span data-stu-id="103f1-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="103f1-111">[การจัดการสิทธิ์ในข้อมูลในสํานักงาน](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span><span class="sxs-lookup"><span data-stu-id="103f1-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="103f1-112">[การจัดการสิทธิ์ในข้อมูลในการแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="103f1-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


