---
title: ลบหรือคืนค่าแอปพลิเคชัน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015020"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="3e13d-102">ลบหรือคืนค่าแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="3e13d-102">Delete or restore applications</span></span>

<span data-ttu-id="3e13d-103">**เมื่อต้องการลบแอปพลิเคชันจากผู้เช่า AZURE AD ของคุณ**:</span><span class="sxs-lookup"><span data-stu-id="3e13d-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="3e13d-104">ใน **พอร์ทัล AD Azure** ให้เลือก **แอปพลิเคชันสำหรับองค์กร**</span><span class="sxs-lookup"><span data-stu-id="3e13d-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="3e13d-105">จากนั้นค้นหาและเลือกแอปพลิเคชันที่คุณต้องการลบ</span><span class="sxs-lookup"><span data-stu-id="3e13d-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="3e13d-106">ในส่วน **จัดการ** ในบานหน้าต่างด้านซ้ายให้เลือก **คุณสมบัติ**</span><span class="sxs-lookup"><span data-stu-id="3e13d-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="3e13d-107">เลือก **ลบ** จากนั้นเลือก **ใช่** เพื่อยืนยันว่าคุณต้องการลบแอปจากผู้เช่า Azure AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="3e13d-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="3e13d-108">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการลบแอปให้ดูที่[Quickstart: ลบแอปพลิเคชันจากผู้เช่า Azure Active directory (AZURE AD) ของคุณ](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="3e13d-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="3e13d-109">ใน PowerShell cmdlet การ [เอา AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) เอาการกำหนดค่าพร็อกซีของแอปพลิเคชันออกจากแอปพลิเคชันที่เฉพาะเจาะจงใน Azure active directory และสามารถลบแอปพลิเคชันทั้งหมดได้ถ้ามีการระบุไว้</span><span class="sxs-lookup"><span data-stu-id="3e13d-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="3e13d-110">คุณสามารถ **คืนค่าแอปพลิเคชันที่ถูกลบ** โดยใช้ PowerShell ได้</span><span class="sxs-lookup"><span data-stu-id="3e13d-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="3e13d-111">เมื่อแอปพลิเคชันที่คุณต้องการคืนค่าได้รับการระบุแล้วคุณสามารถคืนค่าได้โดยใช้การ[คืนค่า-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)</span><span class="sxs-lookup"><span data-stu-id="3e13d-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
