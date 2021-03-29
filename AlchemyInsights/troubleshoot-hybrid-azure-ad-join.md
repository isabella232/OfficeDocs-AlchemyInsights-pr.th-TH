---
title: แก้ไขปัญหาการเข้าร่วม Azure AD แบบไฮบริด
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401926"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="17cdf-102">แก้ไขปัญหาการเข้าร่วม Azure AD แบบไฮบริด</span><span class="sxs-lookup"><span data-stu-id="17cdf-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="17cdf-103">ขอแนะนนะให้ตรวจสอบให้แน่ใจว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบโดยใช้ [สคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)ทดสอบ</span><span class="sxs-lookup"><span data-stu-id="17cdf-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="17cdf-104">ถ้าคุณตั้งค่าการลงทะเบียนอุปกรณ์เป็นครั้งแรก ให้ตรวจสอบให้แน่ใจว่าได้ตรวจทานบทสรุปของการจัดการอุปกรณ์ใน Azure[Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) เพื่อเรียนรู้วิธีรับอุปกรณ์ภายใต้การควบคุมของ Azure AD</span><span class="sxs-lookup"><span data-stu-id="17cdf-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="17cdf-105">หากคุณลงทะเบียนอุปกรณ์ลงใน Azure AD โดยตรง และลงทะเบียนอุปกรณ์เหล่านั้นลงใน Intuned ตรวจสอบให้แน่ใจว่าคุณได้กําหนดค่า[Intuned](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)และได้[](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)ให้สิทธิ์การใช้งานแล้วก่อน</span><span class="sxs-lookup"><span data-stu-id="17cdf-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="17cdf-106">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการใน Azure AD และ AD ภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="17cdf-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="17cdf-107">เฉพาะผู้ดูแลระบบส่วนกลางใน Azure AD เท่านั้นที่สามารถจัดการการตั้งค่าการลงทะเบียนอุปกรณ์ได้</span><span class="sxs-lookup"><span data-stu-id="17cdf-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="17cdf-108">นอกจากนี้ ถ้าคุณตั้งค่าการลงทะเบียนอัตโนมัติใน Active Directory ภายในองค์กรของคุณ คุณจะต้องเป็นผู้ดูแลระบบของ Active Directory และ AD FS (ถ้ามี)</span><span class="sxs-lookup"><span data-stu-id="17cdf-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="17cdf-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see Set up hybrid Azure AD join [(on-premises domain-join) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and Manage devices using the Azure [portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="17cdf-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="17cdf-110">เมื่อต้องการแก้ไขปัญหาทั่วไปเกี่ยวกับการรวม Active Directory (AD) ของ Azure แบบไฮบริด ให้ดู FAQ[การเข้าร่วม Azure AD แบบไฮบริด](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)</span><span class="sxs-lookup"><span data-stu-id="17cdf-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
