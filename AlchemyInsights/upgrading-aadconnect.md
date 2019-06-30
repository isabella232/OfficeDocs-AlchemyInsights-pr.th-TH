---
title: AADConnect การปรับรุ่น 932
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365933"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9f462-102">การเชื่อมต่อ Azure AD การปรับรุ่น</span><span class="sxs-lookup"><span data-stu-id="9f462-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9f462-103">โดยค่าเริ่มต้น การอัพเกรดอัตโนมัติถูกเปิดใช้งานสำหรับการเชื่อมต่อ AD Azure ซึ่งช่วยให้แน่ใจว่าคุณกำลังเรียกใช้รุ่นล่าสุด</span><span class="sxs-lookup"><span data-stu-id="9f462-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="9f462-104">เมื่อต้องการตรวจสอบการตั้งค่าการปรับรุ่นอัตโนมัติ ใช้ cmdlet การ**ADSyncAutoUpgrade รับ**ใน PowerShell โฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="9f462-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="9f462-105">Cmdlet นี้จะส่งกลับค่าหนึ่งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9f462-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="9f462-106">**เปิดการใช้งาน**: เปิดใช้งานการปรับรุ่นโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="9f462-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="9f462-107">**ปิดการใช้งาน**: การอัพเกรดอัตโนมัติถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="9f462-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="9f462-108">**ระงับ**: ระบบไม่มีสิทธิ์ได้รับการปรับรุ่นโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="9f462-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="9f462-109">คุณไม่สามารถกำหนดค่านี้ จะถูกกำหนด โดยระบบ</span><span class="sxs-lookup"><span data-stu-id="9f462-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="9f462-110">สำหรับข้อมูลเพิ่มเติม ดู[การอัพเกรดโดยอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)</span><span class="sxs-lookup"><span data-stu-id="9f462-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="9f462-111">เมื่อต้องการดาวน์โหลดรุ่นล่าสุดของการเชื่อมต่อ AD Azure ไป[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="9f462-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
