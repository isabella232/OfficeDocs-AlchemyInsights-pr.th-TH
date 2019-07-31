---
title: ปัญหาในการลงชื่อเข้าใช้กับโปรแกรมประยุกต์ของ Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938367"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="15226-102">เครื่องหมายในหน้าจอว่างในโปรแกรมประยุกต์ของ Office</span><span class="sxs-lookup"><span data-stu-id="15226-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="15226-103">เมื่อต้องการแก้ไขปัญหานี้ ลองต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="15226-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="15226-104">ติดตั้งโปรแกรมปรับปรุงล่าสุดสำหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="15226-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="15226-105">รีเซ็ตตัวเลือก Internet Explorer: ไปที่**เครื่องมือ** > **ตัวเลือกอินเทอร์เน็ต** > **ขั้นสูง** > **ตั้งค่า Internet Explorer** (โปรดสังเกตว่า คุณจะสูญเสียการตั้งค่าแบบกำหนดเอง), แล้วลองลงชื่อเข้าใช้ให้กับสำนักงานอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="15226-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="15226-106">ปิดการใช้งาน Windows Defender โปรแกรมประยุกต์ Guard (WDAG) หรือโปรแกรมไฟร์วอลล์หรือโปรแกรมป้องกันไวรัสใด ๆ คล้ายกัน:</span><span class="sxs-lookup"><span data-stu-id="15226-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="15226-107">ใน'แผงควบคุม' ไปยัง**โปรแกรม**และจากนั้น เลือก**เปิด หรือปิดคุณลักษณะของ Windows ที่เปิดใช้งาน**</span><span class="sxs-lookup"><span data-stu-id="15226-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="15226-108">ถ้าเปิดใช้งาน Windows Guard แอพลิเคชันของ Defender ลองปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="15226-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="15226-109">**หมายเหตุ:** คุณอาจต้องรีสตาร์ทเครื่องคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="15226-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="15226-110">ให้แน่ใจว่า Microsoft.AAD.BrokerPlugin [WAM AAD ปลั๊กอิน](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)ไม่ถูกบล็อก โดยโปรแกรมประยุกต์หรือไฟร์ วอลล์/anti-virus โปรแกรมใด ๆ</span><span class="sxs-lookup"><span data-stu-id="15226-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="15226-111">[ข้อมูลประจำตัวของ Office ล้าง](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="15226-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="15226-112">**หมายเหตุ:** มีเปลี่ยนเส้นทางรีจิสทรีสำหรับ Office 2016 แปลง 16.0</span><span class="sxs-lookup"><span data-stu-id="15226-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="15226-113">(แลกเปลี่ยน: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="15226-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="15226-114">สำหรับข้อมูลเพิ่มเติม ดู[ปัญหาการเชื่อมต่อในเครื่องหลังจากการปรับปรุง Office 2016 build 16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="15226-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>