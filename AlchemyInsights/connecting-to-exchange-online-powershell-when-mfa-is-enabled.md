---
title: Connecting 761 การแลกเปลี่ยน PowerShell ออนไลน์เมื่อมีการเปิดใช้งาน MFA
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/26/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 761
ms.assetid: 9b0b89e3-d1d7-4e4d-93de-bb4cd00904d8
ms.openlocfilehash: 02c42175df821e17641b4252f5dd267eceb0e508
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753690"
---
# <a name="connect-to-exchange-online-powershell-when-mfa-is-enabled"></a><span data-ttu-id="da684-102">เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนเมื่อมีการเปิดใช้งาน MFA</span><span class="sxs-lookup"><span data-stu-id="da684-102">Connect to Exchange Online PowerShell when MFA is enabled</span></span>

<span data-ttu-id="da684-103">ถ้าบัญชีของคุณได้เปิดใช้งานด้วยหลายปัจจัยการตรวจสอบ (MFA) คุณจำเป็นต้องทำตามคำแนะนำเหล่านี้เพื่อเชื่อมต่อกับ PowerShell ออนไลน์ของ Exchange: [PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนการเชื่อมต่อโดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="da684-103">If your account has multi-factor authentication (MFA) enabled, you need to follow these instructions to connect to Exchange Online PowerShell: [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).</span></span>

<span data-ttu-id="da684-104">**หมายเหตุ**: แม้ว่าคุณได้เชื่อมต่อกับ PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยนในอดีตโดยใช้[คำสั่งการเชื่อมต่อทั่วไป](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)คุณต้องใช้คำแนะนำในการเชื่อมต่อ MFA หลังจาก MFA ได้ถูกเปิดใช้งานสำหรับบัญชีผู้ใช้ของคุณ</span><span class="sxs-lookup"><span data-stu-id="da684-104">**Note**: Even if you've connected to Exchange Online PowerShell in the past using [the regular connection instructions](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell), you need to use the MFA connection instructions after MFA has been enabled for your account.</span></span>
