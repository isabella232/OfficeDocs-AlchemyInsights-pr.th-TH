---
title: เตรียมสําหรับการใช้ TLS 1.2 ใน Microsoft 365
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
ms.openlocfilehash: 4d4206036e293419e4bc2400296ed4b0bd67e0f7
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "43785286"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="49093-102">เตรียมสําหรับการใช้ TLS 1.2 ใน Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="49093-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="49093-103">ณ วันที่ 31 ตุลาคม 2018 Microsoft 365 จะยังคงเปลี่ยนไปเป็น TLS 1.2 ต่อไป</span><span class="sxs-lookup"><span data-stu-id="49093-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="49093-104">ซึ่งหมายความว่า Microsoft จะไม่แก้ไขปัญหาใหม่ที่พบในไคลเอ็นต์ อุปกรณ์ หรือบริการที่เชื่อมต่อกับ Microsoft 365 โดยใช้ TLS 1.0 และ 1.1</span><span class="sxs-lookup"><span data-stu-id="49093-104">This means that Microsoft will not fix new issues that are found in clients, devices, or services that connect to Microsoft 365 by using TLS 1.0 and 1.1.</span></span> <span data-ttu-id="49093-105">**นี้ไม่ได้หมายความว่า Microsoft 365 จะบล็อกการเชื่อมต่อ TLS 1.0 และ 1.1**</span><span class="sxs-lookup"><span data-stu-id="49093-105">**This does not mean Microsoft 365 will block TLS 1.0 and 1.1 connections.**</span></span> <span data-ttu-id="49093-106">วันที่เลิกใช้ขั้นสุดท้ายจะถูกกําหนดโดยการใช้งานของลูกค้าและสถานะปัจจุบันของการรักษาความปลอดภัย TLS แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="49093-106">The eventual deprecation date will be determined by customer usage and the current state of legacy TLS security.</span></span> <span data-ttu-id="49093-107">หลังจากการตัดสินใจแล้วจะมีการประกาศล่วงหน้าหกเดือนเว้นแต่เราจะตระหนักถึงการประนีประนอมที่รู้จักกันซึ่งในกรณีนี้เราอาจจะต้องดําเนินการในเวลาน้อยกว่าหกเดือนเพื่อปกป้องลูกค้าที่ใช้บริการ</span><span class="sxs-lookup"><span data-stu-id="49093-107">After a decision is made, there will be an announcement six months in advance unless we become aware of a known compromise, in which case we may have to act in less than six months to protect customers who use the services.</span></span>
  
<span data-ttu-id="49093-108">ขอแนะนําอย่างยิ่งว่า เซิร์ฟเวอร์และไคลเอ็นต์ที่เชื่อมต่อกับ Microsoft 365 จําเป็นต้องเปิดใช้งาน TLS 1.2 โดยเร็วที่สุด</span><span class="sxs-lookup"><span data-stu-id="49093-108">It is strongly suggested that any servers and clients connecting with Microsoft 365 need to enable TLS 1.2 as soon as possible.</span></span>
  
<span data-ttu-id="49093-109">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การเตรียม TLS 1.2 ใน Microsoft 365](https://support.microsoft.com/help/4057306/preparing-for-tls-1-2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="49093-109">For more information see [Preparing for TLS 1.2 in Microsoft 365.](https://support.microsoft.com/help/4057306/preparing-for-tls-1-2-in-office-365)</span></span>
  