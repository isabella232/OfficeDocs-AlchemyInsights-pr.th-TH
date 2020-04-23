---
title: "932"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766512"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="e3064-102">ปรับรุ่นการเชื่อมต่อ AZURE AD</span><span class="sxs-lookup"><span data-stu-id="e3064-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="e3064-103">โดยค่าเริ่มต้น การปรับรุ่นอัตโนมัติถูกเปิดใช้งานสําหรับ Azure AD Connect ซึ่งช่วยให้คุณมั่นใจว่าคุณกําลังเรียกใช้รุ่นล่าสุด</span><span class="sxs-lookup"><span data-stu-id="e3064-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="e3064-104">เมื่อต้องการตรวจสอบการตั้งค่าการปรับรุ่นอัตโนมัติ**Get-ADSyncAutoUpgrade**</span><span class="sxs-lookup"><span data-stu-id="e3064-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="e3064-105">cmdlet จะส่งกลับค่าต่อไปนี้อย่างใดอย่างหนึ่ง:</span><span class="sxs-lookup"><span data-stu-id="e3064-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="e3064-106">**เปิดใช้งาน**: เปิดใช้งานการปรับรุ่นอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="e3064-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="e3064-107">**ปิดใช้งาน**: การปรับรุ่นอัตโนมัติถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="e3064-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="e3064-108">**ระงับ :** ระบบไม่มีสิทธิ์รับการอัพเกรดอัตโนมัติอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="e3064-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="e3064-109">คุณไม่สามารถกําหนดค่านี้ได้ มันตั้งค่าโดยระบบ</span><span class="sxs-lookup"><span data-stu-id="e3064-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="e3064-110">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การอัพเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)</span><span class="sxs-lookup"><span data-stu-id="e3064-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="e3064-111">เมื่อต้องการดาวน์โหลดการเชื่อมต่อ AD Azure รุ่นล่าสุด ให้ไปที่[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="e3064-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
