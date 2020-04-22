---
title: ปิดการซิงค์ UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726123"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="c34f6-102">ปิดการซิงค์ UPN</span><span class="sxs-lookup"><span data-stu-id="c34f6-102">UPN sync disabled</span></span>

<span data-ttu-id="c34f6-103">ถ้าคุณเริ่มต้นการซิงค์กับ Azure AD ก่อน 30 มีนาคม 2016 เรียกใช้ cmdlet PowerShell โฆษณา Azure ต่อไปนี้เพื่อเปิดใช้งานการจับคู่อ่อน UPN สําหรับองค์กรของคุณเท่านั้น:</span><span class="sxs-lookup"><span data-stu-id="c34f6-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="c34f6-104">**เปิดใช้งานคุณลักษณะ -เปิดใช้งานซอฟต์แมทแมทช์$Trueเปิดใช้งาน$True**</span><span class="sxs-lookup"><span data-stu-id="c34f6-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="c34f6-105">การจับคู่แบบอ่อน UPN จะเปิดโดยอัตโนมัติสําหรับองค์กรที่เริ่มซิงค์กับ Azure AD บน หรือหลังจากวันที่ 30 มีนาคม 2016</span><span class="sxs-lookup"><span data-stu-id="c34f6-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="c34f6-106">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่แบบอ่อนบน UPN และคุณลักษณะการซิงค์อื่น ๆ โปรดดู[คุณลักษณะ Azure AD ซิงค์บริการซิงค์](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="c34f6-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

