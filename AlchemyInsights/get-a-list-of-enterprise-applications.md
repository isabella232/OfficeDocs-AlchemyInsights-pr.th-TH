---
title: ดูรายการของแอปพลิเคชัน Enterprise
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405510"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="f3242-102">ดูรายการแอปพลิเคชันระดับองค์กร</span><span class="sxs-lookup"><span data-stu-id="f3242-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="f3242-103">เมื่อต้องการรับ **รายการ** แอปพลิเคชันขององค์กร (แอปพลิเคชันทั้งหมดหรือกรองตามชื่อที่ใช้แสดง, ID, URI ของตัวระบุ และอื่นๆ) ผ่านสั่ง Powershell ให้ดู [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="f3242-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="f3242-104">เมื่อต้องการรับรายการวัตถุหลักของบริการ (วัตถุทั้งหมดหรือกรองตาม ID) ผ่านสั่ง Powershell ให้ดู[Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="f3242-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="f3242-105">ถ้าคุณต้องการดูรายการ **แอปที่กําหนดค่า SAML สคริปต์ PowerShell ต่อไปนี้** อาจช่วยคุณได้:</span><span class="sxs-lookup"><span data-stu-id="f3242-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="f3242-106">แอปพลิเคชันทั้งหมดจะเป็นแอป OAuth หรือแอป SAML (ทั้งแกลเลอรีและแอปที่ไม่อยู่ในแกลเลอรี) จะมีวัตถุสองรายการที่สร้างขึ้นใน AAD เมื่อการลงทะเบียนของพวกเขาเกิดขึ้น</span><span class="sxs-lookup"><span data-stu-id="f3242-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="f3242-107">วัตถุหนึ่งเรียกว่า วัตถุของแอปพลิเคชัน และอีกวัตถุหนึ่งคือวัตถุ Service Principal</span><span class="sxs-lookup"><span data-stu-id="f3242-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="f3242-108">เมื่อคุณระบุคุณสมบัติของวัตถุหลักบริการโดยใช้ PowerShell คุณจะพบว่าทุกแอปพลิเคชันมีแท็กที่เกี่ยวข้องกับแอปพลิเคชันนั้นจํานวนหนึ่ง ดังนี้</span><span class="sxs-lookup"><span data-stu-id="f3242-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="f3242-109">แอป OAuth จะมีแท็กที่เรียกว่า "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="f3242-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="f3242-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="f3242-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="f3242-111">แอป SAML ที่ไม่ใช่แกลเลอรีจะมีแท็กที่เรียกว่า "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="f3242-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="f3242-112">ดังนั้น คุณสามารถใช้แท็กเหล่านี้และค้นหาชนิดของแอปได้</span><span class="sxs-lookup"><span data-stu-id="f3242-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="f3242-113">แท็ก "**WindowsAzureActiveDirectoryIntegratedApp**" เป็นแอปทุกประเภท</span><span class="sxs-lookup"><span data-stu-id="f3242-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="f3242-114">คุณสามารถใช้ส่วนย่อยต่อไปนี้เพื่อแสดงรายการแอป SAML ทั้งหมด (ทั้งแกลเลอรีและแอปที่ไม่อยู่ในแกลเลอรี):</span><span class="sxs-lookup"><span data-stu-id="f3242-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="f3242-115">ดูข้อมูลเพิ่มเติมในการระบุ[แอปที่เปิดใช้งาน SAML ใน Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="f3242-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="f3242-116">**ค้นหาและแสดงรายการแอปพลิเคชันบนเว็บเท่านั้น**: ใช้สั่งด้านล่างเพื่อรับแอปพลิเคชัน Azure AD ทั้งหมดที่มีประเภทแอปพลิเคชัน "เว็บแอป/API"</span><span class="sxs-lookup"><span data-stu-id="f3242-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="f3242-117">Get-AzureADApplication -ทั้งหมด:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="f3242-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="f3242-118">**ค้นหาและแสดงรายการแอปพลิเคชันดั้งเดิมอย่างเดียว**: เรียกใช้สั่งต่อไปนี้เพื่อรับแอปพลิเคชันไคลเอ็นต์ดั้งเดิม (เดสก์ท็อป/อุปกรณ์เคลื่อนที่) ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="f3242-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="f3242-119">Get-AzureADApplication -ทั้งหมด:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="f3242-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="f3242-120">**ส่งออกรายละเอียดแอปพลิเคชัน Azure AD ที่ลงทะเบียนทั้งหมดเป็น CSV**: ด้านล่างสั่งส่งออกแอป Azure AD ทั้งหมดที่มีรายละเอียดที่ต้องมีไปยังไฟล์ csv:</span><span class="sxs-lookup"><span data-stu-id="f3242-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="f3242-121">Get-AzureADApplication -ทั้งหมด:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="f3242-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="f3242-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="f3242-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="f3242-123">**ต้องการส่งออกรายการแอป Azure ที่ไม่ได้ใช้** – รายงานการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="f3242-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="f3242-124">Azure AD สามารถแสดงบันทึกแอปพลิเคชันได้นานถึง 30 วันที่คุณให้สิทธิ์การใช้งาน Azure AD Premium</span><span class="sxs-lookup"><span data-stu-id="f3242-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="f3242-125">คุณมีสองตัวเลือกในการเก็บข้อมูลไว้นานกว่า 30 วัน</span><span class="sxs-lookup"><span data-stu-id="f3242-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="f3242-126">คุณสามารถใช้ API [การรายงานของ Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) เพื่อเรียกใช้ข้อมูลโดยทางโปรแกรมและจัดเก็บในฐานข้อมูล</span><span class="sxs-lookup"><span data-stu-id="f3242-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="f3242-127">อีกวิธีหนึ่งคือ คุณสามารถรวมบันทึกการตรวจสอบลงในระบบของ PARTY</span><span class="sxs-lookup"><span data-stu-id="f3242-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="f3242-128">คุณยังสามารถดาวน์โหลดรายการแอปของแอปพลิเคชันทั้งหมดและแอปพลิเคชันที่เป็นเจ้าของภายใต้ Azure Active Directory>การลงทะเบียน>ดาวน์โหลด>แอปพลิเคชันทั้งหมด/แอปพลิเคชันที่เป็นเจ้าของ</span><span class="sxs-lookup"><span data-stu-id="f3242-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="f3242-129">เมื่อต้องการรับรายการแอปพลิเคชันผ่าน MS Graph ให้ดูแอปพลิเคชัน[รายการ - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list)และ[ชนิดของทรัพยากรแอปพลิเคชัน - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="f3242-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
