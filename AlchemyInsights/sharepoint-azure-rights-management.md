---
title: จํากัดการเข้าถึงใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 77f9938fe40d9f693ccce1dac3581625ed7e424a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509583"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="f6085-102">การป้องกัน IRM ไปยังแฟ้ม SharePoint</span><span class="sxs-lookup"><span data-stu-id="f6085-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="f6085-103">ภายใน SharePoint Online การป้องกัน IRM จะถูกนําไปใช้กับแฟ้มที่ระดับรายการและไลบรารี</span><span class="sxs-lookup"><span data-stu-id="f6085-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="f6085-104">ก่อนที่องค์กรของคุณจะสามารถใช้การป้องกัน IRM ได้ คุณต้องตั้งค่าการจัดการสิทธิ์ก่อน</span><span class="sxs-lookup"><span data-stu-id="f6085-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="f6085-105">IRM อาศัยบริการการจัดการสิทธิ์ Azure จากการป้องกันข้อมูล Azure เพื่อเข้ารหัสลับ และกําหนดข้อจํากัดการใช้งาน</span><span class="sxs-lookup"><span data-stu-id="f6085-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="f6085-106">การสมัครใช้งาน Microsoft 365 บางอย่างรวมถึงการจัดการสิทธิ์ Azure แต่ไม่ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="f6085-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="f6085-107">หากต้องการเรียนรู้เพิ่มเติม โปรดดู:</span><span class="sxs-lookup"><span data-stu-id="f6085-107">To learn more, see:</span></span>

- <span data-ttu-id="f6085-108">[วิธีที่โปรแกรมประยุกต์และบริการ Office สนับสนุนการจัดการสิทธิ์ Azure](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)</span><span class="sxs-lookup"><span data-stu-id="f6085-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="f6085-109">[ตั้งค่าการจัดการสิทธิ์ในข้อมูล (IRM) ในศูนย์การจัดการ SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center)</span><span class="sxs-lookup"><span data-stu-id="f6085-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="f6085-110">[ไลบรารีเอกสารของ SharePoint ที่เปิดใช้งาน IRM และรายการ](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)</span><span class="sxs-lookup"><span data-stu-id="f6085-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="f6085-111">[การจัดการสิทธิ์ในข้อมูลใน Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span><span class="sxs-lookup"><span data-stu-id="f6085-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="f6085-112">[การจัดการสิทธิ์ในข้อมูลในการแลกเปลี่ยนแบบออนไลน์](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="f6085-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


