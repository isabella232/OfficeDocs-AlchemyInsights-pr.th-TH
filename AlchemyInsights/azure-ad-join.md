---
title: การเข้าร่วม Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405670"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="a9f95-102">การเข้าร่วม Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a9f95-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="a9f95-103">ถ้าคุณตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรก ตรวจสอบให้แน่ใจว่าคุณได้ตรวจทานบทนําสู่การจัดการอุปกรณ์ใน Azure [Active Directory](/azure/active-directory/devices/overview) ที่จะแนะนําวิธีรับอุปกรณ์ภายใต้การควบคุมไปยัง Azure AD</span><span class="sxs-lookup"><span data-stu-id="a9f95-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="a9f95-104">หากคุณลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรง และลงทะเบียนอุปกรณ์เหล่านั้นลงใน Intuned คุณจะต้องตรวจสอบให้แน่ใจว่า คุณได้กําหนดค่า[Intuned](/mem/intune/enrollment/device-enrollment)และมีสิทธิ์การใช้งาน[](/mem/intune/fundamentals/licenses-assign)ก่อน</span><span class="sxs-lookup"><span data-stu-id="a9f95-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="a9f95-105">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการใน Azure AD</span><span class="sxs-lookup"><span data-stu-id="a9f95-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="a9f95-106">เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าการลงทะเบียนอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="a9f95-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="a9f95-107">เมื่อต้องการใช้การเข้าร่วม Azure AD ให้ดู[วางแผนการเข้าร่วม Azure AD](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="a9f95-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="a9f95-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span><span class="sxs-lookup"><span data-stu-id="a9f95-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
