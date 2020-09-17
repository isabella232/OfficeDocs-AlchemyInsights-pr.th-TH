---
title: ๙๓๒การอัปเกรด AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806058"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="51f7a-102">การอัปเกรด Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="51f7a-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="51f7a-103">ตามค่าเริ่มต้นการอัปเกรดอัตโนมัติจะถูกเปิดใช้งานสำหรับ Azure AD Connect ซึ่งจะช่วยให้แน่ใจว่าคุณกำลังใช้งานเวอร์ชันล่าสุด</span><span class="sxs-lookup"><span data-stu-id="51f7a-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="51f7a-104">เมื่อต้องการตรวจสอบการตั้งค่าการอัปเกรดอัตโนมัติให้ใช้ cmdlet **รับ ADSyncAutoUpgrade** ใน PowerShell AD Azure</span><span class="sxs-lookup"><span data-stu-id="51f7a-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="51f7a-105">Cmdlet นี้จะส่งกลับค่าใดค่าหนึ่งดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="51f7a-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="51f7a-106">**เปิดใช้**งาน: เปิดใช้งานการอัปเกรดอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="51f7a-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="51f7a-107">**ปิดใช้**งาน: การอัปเกรดอัตโนมัติถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="51f7a-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="51f7a-108">**ถูกระงับ**: ระบบจะไม่มีสิทธิ์ในการรับการอัปเกรดอัตโนมัติอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="51f7a-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="51f7a-109">คุณไม่สามารถกำหนดค่านี้ได้ ระบบจะตั้งค่าโดยระบบ</span><span class="sxs-lookup"><span data-stu-id="51f7a-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="51f7a-110">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[อัปเกรดอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)</span><span class="sxs-lookup"><span data-stu-id="51f7a-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="51f7a-111">เมื่อต้องการดาวน์โหลดเวอร์ชันล่าสุดของ Azure AD [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) Connect ให้ไปที่</span><span class="sxs-lookup"><span data-stu-id="51f7a-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
