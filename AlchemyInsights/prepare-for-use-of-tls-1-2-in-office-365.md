---
title: การเตรียมพร้อมสําหรับการใช้ TLS 1.2 ใน Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 319a5b089da94c8a2dcf7aef7d9e1bf791490d08
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43666940"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="3e56e-102">การเตรียมพร้อมสําหรับการใช้ TLS 1.2 ใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3e56e-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="3e56e-103">ณ วันที่ 31 ตุลาคม 2018, Microsoft 365 จะดําเนินต่อการเปลี่ยนเป็น TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="3e56e-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="3e56e-104">อุปกรณ์ หรือบริการที่เชื่อมต่อกับ Office 365 โดยใช้ TLS 1.0 และ 1.1</span><span class="sxs-lookup"><span data-stu-id="3e56e-104">This means that Microsoft will not fix new issues that are found in clients, devices, or services that connect to Office 365 by using TLS 1.0 and 1.1.</span></span> <span data-ttu-id="3e56e-105">**นี้ไม่ได้หมายความว่า Microsoft 365 จะบล็อกการเชื่อมต่อ TLS 1.0 และ 1.1**</span><span class="sxs-lookup"><span data-stu-id="3e56e-105">**This does not mean Microsoft 365 will block TLS 1.0 and 1.1 connections.**</span></span> <span data-ttu-id="3e56e-106">วันที่เลิกใช้ที่สุดจะถูกกําหนดโดยการใช้งานของลูกค้าและสถานะปัจจุบันของการรักษาความปลอดภัย TLS ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="3e56e-106">The eventual deprecation date will be determined by customer usage and the current state of legacy TLS security.</span></span> <span data-ttu-id="3e56e-107">หลังจากการตัดสินใจแล้วจะมีการประกาศหกเดือนล่วงหน้าเว้นแต่เราจะตระหนักถึงการประนีประนอมที่รู้จักกันซึ่งในกรณีนี้เราอาจต้องดําเนินการในเวลาน้อยกว่าหกเดือนเพื่อปกป้องลูกค้าที่ใช้บริการ</span><span class="sxs-lookup"><span data-stu-id="3e56e-107">After a decision is made, there will be an announcement six months in advance unless we become aware of a known compromise, in which case we may have to act in less than six months to protect customers who use the services.</span></span>
  
<span data-ttu-id="3e56e-108">ขอแนะนําว่า เซิร์ฟเวอร์และไคลเอนต์เชื่อมต่อกับ Microsoft 365 จําเป็นต้องเปิดใช้งาน TLS 1.2 โดยเร็วที่สุด</span><span class="sxs-lookup"><span data-stu-id="3e56e-108">It is strongly suggested that any servers and clients connecting with Microsoft 365 need to enable TLS 1.2 as soon as possible.</span></span>
  
<span data-ttu-id="3e56e-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การจัดเตรียมสําหรับ TLS 1.2 ใน Microsoft 365](https://support.microsoft.com/help/4057306/preparing-for-tls-1-2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="3e56e-109">For more information see [Preparing for TLS 1.2 in Microsoft 365.](https://support.microsoft.com/help/4057306/preparing-for-tls-1-2-in-office-365)</span></span>
  