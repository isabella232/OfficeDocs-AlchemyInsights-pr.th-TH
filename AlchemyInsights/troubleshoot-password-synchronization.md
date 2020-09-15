---
title: การแก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664945"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="919e6-102">การแก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="919e6-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="919e6-103">เมื่อต้องการแก้ไขปัญหาการซิงโครไนซ์รหัสผ่านให้เริ่มต้นโดยใช้การแก้ไขปัญหา AAD เชื่อมต่อนี้เพื่อกำหนดว่าทำไมรหัสผ่านจึงไม่ได้รับการซิงค์</span><span class="sxs-lookup"><span data-stu-id="919e6-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="919e6-104">เมื่อต้องการเริ่มต้นให้ไปที่[จัดการการซิงค์โดยตรง](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)</span><span class="sxs-lookup"><span data-stu-id="919e6-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="919e6-105">เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์ Azure AD Connect ของคุณแล้วเลือกตัวเลือก**เรียกใช้ในฐานะผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="919e6-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="919e6-106">เรียกใช้การตั้งค่า-ExecutionPolicy RemoteSigned หรือตั้งค่า ExecutionPolicy ไม่จำกัด</span><span class="sxs-lookup"><span data-stu-id="919e6-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="919e6-107">เริ่มตัวช่วยสร้างการเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="919e6-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="919e6-108">ไปที่หน้างานเพิ่มเติม >**แก้ไขปัญหา**  >  **ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="919e6-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="919e6-109">เลือก **เปิด** ใช้เพื่อเปิดเมนูการแก้ไขปัญหา PowerShell</span><span class="sxs-lookup"><span data-stu-id="919e6-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="919e6-110">เลือก**แก้ไขปัญหาการซิงโครไนซ์รหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="919e6-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="919e6-111">ปัญหานี้มักจะเป็นการซิงโครไนซ์รหัสผ่านสำหรับบัญชีผู้ใช้ที่เฉพาะเจาะจง</span><span class="sxs-lookup"><span data-stu-id="919e6-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="919e6-112">**บันทึกย่อ** การซิงโครไนซ์รหัสผ่านล้มเหลวถ้าการซิงค์รหัสผ่านที่เสร็จสมบูรณ์ล่าสุดเป็นเวลาที่แล้ว</span><span class="sxs-lookup"><span data-stu-id="919e6-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="919e6-113">สำหรับความช่วยเหลือเพิ่มเติมในการแก้ไขปัญหาการซิงโครไนซ์รหัสผ่านให้ดู[แก้ไขปัญหาการซิงโครไนซ์แฮชของรหัสผ่านด้วย AZURE AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="919e6-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>