---
title: 761การเชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อเปิดใช้งาน MFA
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "761"
- "3500011"
ms.assetid: 9b0b89e3-d1d7-4e4d-93de-bb4cd00904d8
ms.openlocfilehash: 81d9e74652b20d2bbae6cae581cc31fdc33e82da
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705824"
---
# <a name="connect-to-exchange-online-powershell-when-mfa-is-enabled"></a><span data-ttu-id="145ee-102">เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อเปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="145ee-102">Connect to Exchange Online PowerShell when MFA is enabled</span></span>

<span data-ttu-id="145ee-103">ถ้าบัญชีของคุณมีการเปิดใช้งานการรับรองความถูกต้องด้วยหลายปัจจัย (MFA) คุณจําเป็นต้องทําตามคําแนะนําเหล่านี้เพื่อเชื่อมต่อกับ PowerShell แบบออนไลน์[ของอัตราแลกเปลี่ยน: เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="145ee-103">If your account has multi-factor authentication (MFA) enabled, you need to follow these instructions to connect to Exchange Online PowerShell: [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).</span></span>

<span data-ttu-id="145ee-104">**หมายเหตุ**: แม้ว่าคุณจะเชื่อมต่อกับ Exchange Online PowerShell ในอดีตโดยใช้[คําแนะนําการเชื่อมต่อปกติ](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)คุณต้องใช้คําแนะนําการเชื่อมต่อ MFA หลังจากที่ MFA ได้รับการเปิดใช้งานสําหรับบัญชีของคุณ</span><span class="sxs-lookup"><span data-stu-id="145ee-104">**Note**: Even if you've connected to Exchange Online PowerShell in the past using [the regular connection instructions](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell), you need to use the MFA connection instructions after MFA has been enabled for your account.</span></span>
