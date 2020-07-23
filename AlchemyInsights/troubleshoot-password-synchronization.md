---
title: การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387896"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="ab3e9-102">การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="ab3e9-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="ab3e9-103">เมื่อต้องการแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน ให้เริ่มโดยใช้งานการแก้ไขปัญหาการเชื่อมต่อ AAD นี้เพื่อตรวจสอบว่าเหตุใดรหัสผ่านจึงไม่ซิงค์</span><span class="sxs-lookup"><span data-stu-id="ab3e9-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="ab3e9-104">เมื่อต้องการเริ่มต้น ให้ไปที่[จัดการการซิงค์โดยตรง](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)</span><span class="sxs-lookup"><span data-stu-id="ab3e9-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="ab3e9-105">เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์เชื่อมต่อโฆษณา Azure ของคุณ และเลือกตัวเลือก**เรียกใช้ในฐานะผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="ab3e9-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="ab3e9-106">เรียกใช้ชุดการดําเนินการระยะไกลPolicyหรือตั้งค่า-ExecutionPolicyไม่จํากัด</span><span class="sxs-lookup"><span data-stu-id="ab3e9-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="ab3e9-107">เริ่มตัวช่วยสร้างการเชื่อมต่อโฆษณา Azure</span><span class="sxs-lookup"><span data-stu-id="ab3e9-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="ab3e9-108">ไปที่หน้า งานเพิ่มเติม >**แก้ไขปัญหา**  >  **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="ab3e9-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="ab3e9-109">เลือก**เปิดใช้**เพื่อเปิดเมนูการแก้ไขปัญหา PowerShell</span><span class="sxs-lookup"><span data-stu-id="ab3e9-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="ab3e9-110">เลือก**แก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="ab3e9-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="ab3e9-111">ปัญหานี้มักจะว่า รหัสผ่านจะไม่ซิงโครไนส์สําหรับบัญชีผู้ใช้ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="ab3e9-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="ab3e9-112">**หมายเหตุ** การซิงโครไนส์รหัสผ่านล้มเหลวถ้าการซิงค์รหัสผ่านที่สําเร็จครั้งล่าสุดคือเวลาที่ผ่านมา</span><span class="sxs-lookup"><span data-stu-id="ab3e9-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="ab3e9-113">สําหรับความช่วยเหลือเพิ่มเติมการแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน ให้ดูที่[การแก้ไขปัญหาการซิงโครไนส์แฮชรหัสผ่านด้วยการซิงค์การเชื่อมต่อ AD Azure](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="ab3e9-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>