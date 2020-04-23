---
title: การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732529"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="572c8-102">การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="572c8-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="572c8-103">เมื่อต้องการแก้ไขปัญหาที่ไม่มีรหัสผ่านจะซิงโครไนส์กับ Azure AD Connect รุ่น 1.1.614.0 หรือรุ่นที่ใหม่กว่า:</span><span class="sxs-lookup"><span data-stu-id="572c8-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="572c8-104">เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์ Azure AD Connect ของคุณด้วย**การเรียกใช้ในฐานะผู้ดูแล**ตัวเลือก</span><span class="sxs-lookup"><span data-stu-id="572c8-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="572c8-105">เรียกใช้**ชุด ExecutionPolicy RemoteSigned**หรือ**ชุด ExecutionPolicy ไม่ จํากัด**</span><span class="sxs-lookup"><span data-stu-id="572c8-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="572c8-106">เริ่มตัวช่วยสร้างการเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="572c8-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="572c8-107">นําทางไปยังหน้า**งานเพิ่มเติม\*\*\*\*Troubleshoot\*\*\*\*Next**</span><span class="sxs-lookup"><span data-stu-id="572c8-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="572c8-108">บนหน้า การแก้ไขปัญหา ให้คลิก**เปิดใช้ เพื่อเริ่มเมนูการแก้ไขปัญหา**ใน PowerShell</span><span class="sxs-lookup"><span data-stu-id="572c8-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="572c8-109">ในเมนูหลัก**ให้เลือก**</span><span class="sxs-lookup"><span data-stu-id="572c8-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="572c8-110">ในเมนูย่อย ให้เลือก**การซิงโครไนซ์รหัสผ่าน ไม่ทํางานเลย**</span><span class="sxs-lookup"><span data-stu-id="572c8-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="572c8-111">**ทําความเข้าใจผลลัพธ์ของงานการแก้ไขปัญหา**</span><span class="sxs-lookup"><span data-stu-id="572c8-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="572c8-112">งานการแก้ไขปัญหาทําการตรวจสอบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="572c8-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="572c8-113">ตรวจสอบว่า เปิดใช้งานคุณลักษณะการซิงโครไนส์รหัสผ่านสําหรับผู้เช่า Azure AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="572c8-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="572c8-114">ตรวจสอบว่า เซิร์ฟเวอร์เชื่อมต่อ AD Azure ไม่ได้อยู่ในโหมดการจัดเตรียม</span><span class="sxs-lookup"><span data-stu-id="572c8-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="572c8-115">สําหรับแต่ละตัวเชื่อมต่อ Active Directory ที่มีอยู่ในสถานที่ (ซึ่งสอดคล้องกับฟอเรสต์ Active Directory ที่มีอยู่):</span><span class="sxs-lookup"><span data-stu-id="572c8-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="572c8-116">ตรวจสอบว่าเปิดใช้งานคุณลักษณะการซิงโครไนส์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="572c8-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="572c8-117">ค้นหาเหตุการณ์ heartbeat ฮาร์ทบีทรหัสผ่านในบันทึกเหตุการณ์ของโปรแกรมประยุกต์ Windows</span><span class="sxs-lookup"><span data-stu-id="572c8-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="572c8-118">สําหรับแต่ละโดเมน Active Directory ภายใต้ตัวเชื่อมต่อ Active Directory ในสถาน:</span><span class="sxs-lookup"><span data-stu-id="572c8-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="572c8-119">ตรวจสอบว่า โดเมนสามารถเข้าถึงได้จากเซิร์ฟเวอร์การเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="572c8-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="572c8-120">ตรวจสอบว่า บัญชีบริการระบบโดเมนไดเรกทอรีที่ใช้งานอยู่ (AD DS) ที่ใช้โดยตัวเชื่อมต่อ Active Directory ในสถานที่มีชื่อผู้ใช้ รหัสผ่าน และสิทธิ์ที่ถูกต้องที่จําเป็นสําหรับการซิงโครไนส์ของรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="572c8-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="572c8-121">สําหรับความช่วยเหลือเพิ่มเติมในการแก้ไขปัญหาการซิงค์รหัสผ่าน ให้ดูที่[การแก้ไขปัญหาการซิงค์รหัสผ่านกับการซิงค์ Ad Connect ของ Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)</span><span class="sxs-lookup"><span data-stu-id="572c8-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  