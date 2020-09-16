---
title: ปิดใช้งานการซิงค์ UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749533"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="dc48b-102">ปิดใช้งานการซิงค์ UPN</span><span class="sxs-lookup"><span data-stu-id="dc48b-102">UPN sync disabled</span></span>

<span data-ttu-id="dc48b-103">ถ้าคุณเริ่มการซิงค์กับ Azure AD ก่อนวันที่30มีนาคม๒๐๑๖ให้เรียกใช้ cmdlet PowerShell AD Azure ต่อไปนี้เพื่อเปิดใช้งานการจับคู่นุ่มนวลสำหรับองค์กรของคุณเท่านั้น:</span><span class="sxs-lookup"><span data-stu-id="dc48b-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="dc48b-104">**ตั้งค่า MsolDirSyncFeature-เปิดใช้งาน EnableSoftMatchOnUpn-เปิดใช้งาน $True**</span><span class="sxs-lookup"><span data-stu-id="dc48b-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="dc48b-105">การจับคู่แบบนุ่มของ UPN จะเปิดใช้งานโดยอัตโนมัติสำหรับองค์กรที่เริ่มการซิงค์กับ Azure AD ในหรือหลังวันที่30มีนาคม๒๐๑๖</span><span class="sxs-lookup"><span data-stu-id="dc48b-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="dc48b-106">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการเปิดใช้งานการจับคู่นุ่มบน UPN และฟีเจอร์การซิงค์อื่นๆโปรดดูที่[ฟีเจอร์บริการการซิงค์ AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="dc48b-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

