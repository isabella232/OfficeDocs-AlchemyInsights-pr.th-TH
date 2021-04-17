---
title: เชื่อมต่อกับมอดูล MSCommerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829755"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="140a7-102">MSCommerce ต้องใช้บัญชีของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="140a7-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="140a7-103">โมดูล MSCommerce ต้องใช้บัญชีที่มีสิทธิ์ผู้ดูแลระบบของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="140a7-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="140a7-104">ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้ คุณจะต้องเชื่อมต่อกับบัญชีอื่นอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="140a7-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="140a7-105">*ErrorMessage - เซิร์ฟเวอร์ระยะไกลส่งกลับข้อผิดพลาด: (403) Forbidden ErrorDetails - ที่ C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="140a7-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="140a7-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "ไม่สามารถลองใหม่...*</span><span class="sxs-lookup"><span data-stu-id="140a7-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="140a7-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="140a7-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="140a7-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : ไม่ระบุ: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="140a7-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="140a7-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="140a7-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="140a7-110">ถ้าบัญชีของคุณไม่มีสิทธิ์ผู้ดูแลระบบของบริษัทหรือผู้ดูแลการเรียกเก็บเงิน ให้ติดต่อผู้ดูแลระบบ IT ของคุณ</span><span class="sxs-lookup"><span data-stu-id="140a7-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
