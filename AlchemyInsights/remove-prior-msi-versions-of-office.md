---
title: เอา Office เวอร์ชันก่อนหน้านี้ออกจาก MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680778"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="daae5-102">เอา Office เวอร์ชันก่อนหน้านี้ออกจาก MSI</span><span class="sxs-lookup"><span data-stu-id="daae5-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="daae5-103">ฉันขอแนะนำให้เอา Office Installer (MSI) เวอร์ชันก่อนหน้าก่อนที่จะติดตั้ง Office ๓๖๕ ProPlus</span><span class="sxs-lookup"><span data-stu-id="daae5-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="daae5-104">ต่อไปนี้เป็นวิธีการทำสิ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="daae5-104">Here's how to do this:</span></span>

1. <span data-ttu-id="daae5-105">ถ้าคุณใช้ MSI ในการติดตั้ง Office คุณสามารถใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อถอนการติดตั้ง Office ได้</span><span class="sxs-lookup"><span data-stu-id="daae5-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="daae5-106">คุณสามารถใช้องค์ประกอบ RemoveMSI ในไฟล์ **configuration.xml** ของคุณได้</span><span class="sxs-lookup"><span data-stu-id="daae5-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="daae5-107">ทำตามคำแนะนำในบทความนี้: [ศูนย์การรักษาความปลอดภัย & Office ๓๖๕](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="daae5-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>