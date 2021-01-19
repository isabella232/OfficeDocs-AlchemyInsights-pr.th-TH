---
title: ข้อผิดพลาดในการเข้าสู่ระบบของผู้ใช้
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901251"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="04865-102">ข้อผิดพลาดในการเข้าสู่ระบบของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="04865-102">User sign-in errors</span></span>

<span data-ttu-id="04865-103">**แก้ไขปัญหาเกี่ยวกับการวินิจฉัยการเข้าสู่ระบบ**</span><span class="sxs-lookup"><span data-stu-id="04865-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="04865-104">เมื่อต้องการตรวจหาสาเหตุหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="04865-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="04865-105">เปิดใช้งานการ[วินิจฉัยการลงชื่อเข้าใช้](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="04865-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="04865-106">ค้นหาเหตุการณ์ในการวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้แอปพลิเคชันเวลาของการลงชื่อเข้าใช้ Id คำขอหรือ Id สหสัมพันธ์</span><span class="sxs-lookup"><span data-stu-id="04865-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="04865-107">ตรวจทานผลลัพธ์การวินิจฉัยแสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดำเนินการที่คุณสามารถทำได้เพื่อทำการเปลี่ยนแปลงถ้าจำเป็นต้องมีการเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="04865-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="04865-108">**กำลังมองหาข้อมูลเกี่ยวกับรหัสข้อผิดพลาด AADSTS ที่ส่งกลับจาก Azure Active Directory (Azure AD) token service (STS) ใช่หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="04865-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="04865-109">อ่าน [บทความนี้](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) เพื่อค้นหาคำอธิบายข้อผิดพลาด AADSTS การแก้ไขและการแก้ไขปัญหาบางอย่างที่แนะนำ</span><span class="sxs-lookup"><span data-stu-id="04865-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>