---
title: ซิงค์ UPN ที่ถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657990"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="61d5a-102">ซิงค์ UPN ที่ถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="61d5a-102">UPN sync disabled</span></span>

<span data-ttu-id="61d5a-103">ถ้าคุณเริ่มต้นทำการซิงค์กับโฆษณา Azure ก่อน 30 มีนาคม 2016 เรียกใช้ cmdlet PowerShell โฆษณา Azure ต่อไปนี้เพื่อเปิดใช้งานการจับคู่นุ่ม UPN สำหรับองค์กรของคุณเท่านั้น:</span><span class="sxs-lookup"><span data-stu-id="61d5a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="61d5a-104">**ชุด MsolDirSyncFeature-คุณลักษณะ EnableSoftMatchOnUpn-$True การเปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="61d5a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="61d5a-105">จับคู่นุ่ม UPN จะเปิดโดยอัตโนมัติสำหรับองค์กรที่เริ่มซิงค์ Azure โฆษณาใน หรือหลัง จากวันที่ 30 มีนาคม 2016</span><span class="sxs-lookup"><span data-stu-id="61d5a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="61d5a-106">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่นุ่ม UPN และคุณลักษณะการซิงค์อื่น ๆ โปรดดู[ลักษณะการทำงานการบริการซิงค์เชื่อมต่อ AD Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="61d5a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

