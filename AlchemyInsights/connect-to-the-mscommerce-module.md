---
title: เชื่อมต่อกับโมดู MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3528"
ms.openlocfilehash: 41dd044d99d14f25ea15699bfb74f7c37e3928c1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713257"
---
# <a name="connect-to-the-mscommerce-module"></a><span data-ttu-id="40aad-102">เชื่อมต่อกับโมดู MSCommerce</span><span class="sxs-lookup"><span data-stu-id="40aad-102">Connect to the MSCommerce module</span></span>

<span data-ttu-id="40aad-103">คุณต้องเชื่อมต่อกับโมดู MSCommerce ก่อนที่คุณจะสามารถดูหรือตั้งค่านโยบาย AllowSelfServicePurchase ได้</span><span class="sxs-lookup"><span data-stu-id="40aad-103">You must be connected to the MSCommerce module before you can view or set the AllowSelfServicePurchase policy.</span></span>  

<span data-ttu-id="40aad-104">เมื่อต้องการเชื่อมต่อกับโมดู MSCommerce ที่พร้อมท์ PowerShell (PS C: \) ให้ใส่คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="40aad-104">To connect to the MSCommerce module, at the PowerShell prompt (PS C:\), enter the following command:</span></span>

`Connect-MSCommerce`

<span data-ttu-id="40aad-105">การทำเช่นนี้จะเปิดกล่องโต้ตอบการลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="40aad-105">This will open a sign-in dialog.</span></span> <span data-ttu-id="40aad-106">ใส่ชื่อผู้ใช้และรหัสผ่านของคุณเพื่อลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="40aad-106">Enter your username and password to sign-in.</span></span>

<span data-ttu-id="40aad-107">**หมายเหตุ:** &nbsp; &nbsp; บัญชีผู้ใช้ที่ใช้ในการลงชื่อเข้าใช้ต้องเป็นบริษัทหรือผู้ดูแลระบบการเรียกเก็บเงิน</span><span class="sxs-lookup"><span data-stu-id="40aad-107">**NOTE:**&nbsp;&nbsp;The account used to sign in must be a Company or Billing Administrator.</span></span>
