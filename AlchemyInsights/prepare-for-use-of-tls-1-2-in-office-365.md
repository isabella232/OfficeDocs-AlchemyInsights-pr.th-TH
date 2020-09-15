---
title: เตรียมพร้อมสำหรับการใช้งาน TLS ๑.๒ใน Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 3e1e19c6198cade36930e16445250254e2e50f5e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693977"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="37229-102">เตรียมพร้อมสำหรับการใช้งาน TLS ๑.๒ใน Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="37229-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="37229-103">ณวันที่31ตุลาคม๒๐๑๘ Microsoft ๓๖๕จะดำเนินการเปลี่ยนไปยัง TLS ๑.๒ต่อไป</span><span class="sxs-lookup"><span data-stu-id="37229-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="37229-104">ซึ่งหมายความว่า Microsoft จะไม่แก้ไขปัญหาใหม่ที่พบในไคลเอ็นต์อุปกรณ์หรือบริการที่เชื่อมต่อกับ Microsoft ๓๖๕โดยใช้ TLS ๑.๐และ๑.๑</span><span class="sxs-lookup"><span data-stu-id="37229-104">This means that Microsoft will not fix new issues that are found in clients, devices, or services that connect to Microsoft 365 by using TLS 1.0 and 1.1.</span></span> <span data-ttu-id="37229-105">**นี่ไม่ใช่ Microsoft ๓๖๕จะบล็อกการเชื่อมต่อ TLS ๑.๐และ๑.๑**</span><span class="sxs-lookup"><span data-stu-id="37229-105">**This does not mea Microsoft 365 will block TLS 1.0 and 1.1 connections.**</span></span> <span data-ttu-id="37229-106">วันที่สุดกระท่อมแผนจะถูกกำหนดโดยการใช้งานของลูกค้าและสถานะปัจจุบันของการรักษาความปลอดภัย TLS ดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="37229-106">The eventual deprecation date will be determined by customer usage and the current state of legacy TLS security.</span></span> <span data-ttu-id="37229-107">หลังจากที่มีการตัดสินใจแล้วจะมีการประกาศหกเดือนล่วงหน้าเว้นแต่ว่าเราจะตระหนักถึงการประนีประนอมที่รู้จักซึ่งในกรณีที่เราอาจต้องดำเนินการให้น้อยกว่าหกเดือนเพื่อปกป้องลูกค้าที่ใช้บริการ</span><span class="sxs-lookup"><span data-stu-id="37229-107">After a decision is made, there will be an announcement six months in advance unless we become aware of a known compromise, in which case we may have to act in less than six months to protect customers who use the services.</span></span>
  
<span data-ttu-id="37229-108">ขอแนะนำว่าเซิร์ฟเวอร์และไคลเอ็นต์ใดๆที่เชื่อมต่อกับ Microsoft ๓๖๕จำเป็นต้องเปิดใช้งาน TLS ๑.๒โดยเร็วที่สุดเท่าที่จะเป็นไปได้</span><span class="sxs-lookup"><span data-stu-id="37229-108">It is strongly suggested that any servers and clients connecting with Microsoft 365 need to enable TLS 1.2 as soon as possible.</span></span>
  
<span data-ttu-id="37229-109">สำหรับข้อมูลเพิ่มเติมให้ดู [ที่การเตรียมการสำหรับ TLS ๑.๒ใน Microsoft ๓๖๕](https://support.microsoft.com/help/4057306/preparing-for-tls-1-2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="37229-109">For more information see [Preparing for TLS 1.2 in Microsoft 365.](https://support.microsoft.com/help/4057306/preparing-for-tls-1-2-in-office-365)</span></span>
  