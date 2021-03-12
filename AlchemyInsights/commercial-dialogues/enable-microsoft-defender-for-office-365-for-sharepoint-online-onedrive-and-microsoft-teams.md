---
title: เปิดใช้งาน Microsoft Defender for Office 365 for SharePoint Online, OneDrive และ Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747738"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="26d6a-102">เปิดใช้งาน Microsoft Defender for Office 365 for SharePoint Online, OneDrive และ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="26d6a-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="26d6a-103">ใช้ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยของคุณ เข้าสู่ระบบศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายของ[Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="26d6a-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="26d6a-104">เลือก **การจัดการ** ภัยคุกคามในบานหน้าต่างด้านซ้าย จากนั้นเลือก  >  [นโยบายสิ่งที่แนบมา](https://protection.office.com/safeattachment)ที่ปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="26d6a-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="26d6a-105">เลือก **เปิด Microsoft Defender for Office 365 for SharePoint, OneDrive** และ Microsoft Teams **จากนั้นเลือก** บันทึก</span><span class="sxs-lookup"><span data-stu-id="26d6a-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="26d6a-106">ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet PowerShell ต่อไปนี้ด้วยพารามิเตอร์ **DisallowInfectedFileDownload** ถูกตั้งค่า *เป็น true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="26d6a-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="26d6a-107">ตั้งค่าการแจ้งเตือนไฟล์ที่ถูกตรวจพบ</span><span class="sxs-lookup"><span data-stu-id="26d6a-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="26d6a-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="26d6a-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
