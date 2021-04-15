---
title: การซิงค์ UPN ถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782170"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="7db33-102">การซิงค์ UPN ถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7db33-102">UPN sync disabled</span></span>

<span data-ttu-id="7db33-103">ถ้าคุณเริ่มซิงค์กับ Azure AD ก่อนวันที่ 30 มีนาคม 2016 ให้เรียกใช้ cmdlet PowerShell ของ Azure AD ต่อไปนี้เพื่อเปิดใช้งานการจับคู่ UPN ชั่วคราวให้กับองค์กรของคุณเท่านั้น:</span><span class="sxs-lookup"><span data-stu-id="7db33-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="7db33-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -เปิดใช้งาน$True**</span><span class="sxs-lookup"><span data-stu-id="7db33-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="7db33-105">การจับคู่แบบ UPN จะเปิดใช้งานโดยอัตโนมัติในองค์กรที่เริ่มการซิงค์กับ Azure AD ในหรือหลังวันที่ 30 มีนาคม 2016</span><span class="sxs-lookup"><span data-stu-id="7db33-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="7db33-106">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่แบบ Soft บน UPN และฟีเจอร์การซิงค์อื่นๆ โปรดดู ฟีเจอร์บริการ[การซิงค์ Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="7db33-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

