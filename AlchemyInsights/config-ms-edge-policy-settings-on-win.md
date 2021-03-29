---
title: กําหนดการตั้งค่านโยบายของ Microsoft Edge บน Windows
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
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402394"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="9fc89-102">กําหนดการตั้งค่านโยบายของ Microsoft Edge บน Windows</span><span class="sxs-lookup"><span data-stu-id="9fc89-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="9fc89-103">เมื่อต้องการกําหนดค่าการตั้งค่านโยบายและการอัปเดตที่มีการจัดการของ Microsoft Edge ให้ใช้ Group Policy Objects (GPOs)</span><span class="sxs-lookup"><span data-stu-id="9fc89-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="9fc89-104">คุณยังสามารถเตรียมใช้งานนโยบายผ่านทางรีจิสทรี ซึ่งเหมาะสมกับอุปกรณ์ Windows (1) ที่เข้าร่วมโดเมน Microsoft Active Directory และอินสแตนซ์ Windows 10 Pro และ Enterprise (2) ที่ลงทะเบียนไว้เพื่อการจัดการอุปกรณ์ใน Microsoft Intuned</span><span class="sxs-lookup"><span data-stu-id="9fc89-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="9fc89-105">เมื่อต้องการกําหนดค่า Microsoft Edge โดยใช้ GPOs ให้ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9fc89-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="9fc89-106">ไปที่ Store ส่วนกลางของนโยบายกลุ่ม ในโดเมน Active Directory ของคุณ หรือไปยังโฟลเดอร์เทมเพลตข้อนิยามนโยบายบนคอมพิวเตอร์แต่ละเครื่อง ติดตั้งเทมเพลตการดูแลระบบทั้งหมดที่เพิ่มกฎและการตั้งค่าให้กับ Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9fc89-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="9fc89-107">กําหนดค่านโยบายเฉพาะที่คุณต้องการตั้งค่า</span><span class="sxs-lookup"><span data-stu-id="9fc89-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="9fc89-108">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[กําหนดการตั้งค่านโยบายของ Microsoft Edge บน Windows](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="9fc89-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
