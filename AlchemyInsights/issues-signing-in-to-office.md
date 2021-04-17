---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833058"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="384fd-102">หน้าจอลงชื่อเข้าใช้เปล่าในแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="384fd-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="384fd-103">เมื่อต้องการแก้ไขปัญหานี้ ให้ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="384fd-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="384fd-104">ติดตั้งการอัปเดตล่าสุดของ[Windows](https://support.microsoft.com/help/4027667/windows-10-update) [และ Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="384fd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="384fd-105">ตั้งค่าตัวเลือก Internet Explorer ใหม่:**ไปที่** เครื่องมือ ตัวเลือกอินเทอร์เน็ต ตั้งค่าการตั้งค่า Internet Explorer ใหม่ขั้นสูง (โปรดทราบว่าคุณจะสูญเสียการตั้งค่าแบบปรับแต่งเอง)  >    >    >  แล้วลองลงชื่อเข้าใช้ Office อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="384fd-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="384fd-106">ปิดใช้งาน Windows Defender Application Guard (WDAG) หรือไฟร์วอลล์หรือโปรแกรมป้องกันไวรัสที่คล้ายกัน:</span><span class="sxs-lookup"><span data-stu-id="384fd-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="384fd-107">ใน แผงควบคุม **ให้ไปที่** โปรแกรม แล้วเลือก **เปิดหรือปิดคุณลักษณะ** ของ Windows</span><span class="sxs-lookup"><span data-stu-id="384fd-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="384fd-108">หากเปิดใช้งาน Windows Defender Application Guard ให้ลองปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="384fd-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="384fd-109">**หมายเหตุ:** คุณอาจต้องรีสตาร์ตคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="384fd-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="384fd-110">ตรวจสอบให้แน่ใจว่าปลั๊กอิน [AAD WAM ของ](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft.AAD.BrokerPlugin จะไม่ถูกบล็อกโดยแอปพลิเคชันหรือไฟร์วอลล์/โปรแกรมป้องกันไวรัส</span><span class="sxs-lookup"><span data-stu-id="384fd-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="384fd-111">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="384fd-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="384fd-112">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="384fd-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="384fd-113">(เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="384fd-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="384fd-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="384fd-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>