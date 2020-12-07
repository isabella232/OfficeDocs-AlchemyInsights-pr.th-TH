---
title: การกำหนดค่าการตั้งค่านโยบาย Microsoft Edge บน Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583747"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="da88b-102">การกำหนดค่าการตั้งค่านโยบาย Microsoft Edge บน Windows</span><span class="sxs-lookup"><span data-stu-id="da88b-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="da88b-103">เมื่อต้องการกำหนดค่าการตั้งค่านโยบายและการปรับปรุงที่มีการจัดการสำหรับ Microsoft Edge ให้ใช้วัตถุนโยบายกลุ่ม (GPOs)</span><span class="sxs-lookup"><span data-stu-id="da88b-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="da88b-104">นอกจากนี้คุณยังสามารถจัดเตรียมนโยบายผ่านรีจิสทรีได้อีกด้วย การทำเช่นนี้จะเหมาะสมสำหรับอุปกรณ์ Windows (1) ที่เข้าร่วมกับโดเมน active Directory ของ Microsoft และสำหรับ (2) Windows 10 Pro และอินสแตนซ์ขององค์กรที่ลงทะเบียนสำหรับการจัดการอุปกรณ์ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="da88b-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="da88b-105">เมื่อต้องการกำหนดค่า Microsoft Edge โดยใช้ Gpo ให้ทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="da88b-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="da88b-106">เมื่อต้องการจัดเก็บศูนย์กลางของนโยบายกลุ่มในโดเมน Active Directory ของคุณหรือไปยังโฟลเดอร์เทมเพลตคำนิยามนโยบายบนคอมพิวเตอร์แต่ละเครื่องให้ติดตั้งแม่แบบการดูแลระบบทั้งหมดที่เพิ่มกฎและการตั้งค่าสำหรับ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="da88b-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="da88b-107">กำหนดค่านโยบายเฉพาะที่คุณต้องการตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="da88b-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="da88b-108">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[กำหนดค่าการตั้งค่านโยบาย Microsoft Edge บน Windows](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="da88b-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
