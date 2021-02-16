---
title: Device Writeback
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
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256971"
---
# <a name="device-writeback"></a><span data-ttu-id="56c39-102">Device Writeback</span><span class="sxs-lookup"><span data-stu-id="56c39-102">Device Writeback</span></span>

<span data-ttu-id="56c39-103">ใช้ Device Writeback ในสถานการณ์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="56c39-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="56c39-104">เปิดใช้งาน [Windows Hello for Business โดยใช้การปรับใช้ใบรับรองความเชื่อถือแบบไฮบริด](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="56c39-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="56c39-105">เปิดใช้งานการเข้าถึงตามเงื่อนไขโดยยึดตามอุปกรณ์ไปยังแอปพลิเคชันที่ได้รับการป้องกัน ADFS (2012 R2 หรือสูงกว่า) (ใช้ความน่าเชื่อถือของบริษัท)</span><span class="sxs-lookup"><span data-stu-id="56c39-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="56c39-106">การสมัครใช้งาน Azure AD Premium จะต้องใช้ในการเขียนข้อมูลอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="56c39-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="56c39-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span><span class="sxs-lookup"><span data-stu-id="56c39-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="56c39-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and Setting up [On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="56c39-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="56c39-109">For more information on Enableing Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span><span class="sxs-lookup"><span data-stu-id="56c39-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
