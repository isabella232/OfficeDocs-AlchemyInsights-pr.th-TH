---
title: ปัญหาในการลงชื่อเข้าใช้แอป Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695306"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="79379-102">หน้าจอการลงชื่อเข้าใช้เปล่าในแอป Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="79379-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="79379-103">เมื่อต้องการแก้ไขปัญหานี้ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="79379-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="79379-104">ติดตั้งการอัปเดตล่าสุดสำหรับ[Windows](https://support.microsoft.com/help/4027667/windows-10-update)และ[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="79379-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="79379-105">ตั้งค่าตัวเลือก internet explorer ใหม่: ไปที่**เครื่องมือ**  >  **ตัวเลือก**  >  **Advanced**  >  **การตั้งค่า internet explorer**ขั้นสูงตั้งค่าใหม่ (โปรดทราบว่าคุณจะสูญเสียการตั้งค่าแบบกำหนดเอง) แล้วลองลงชื่อเข้าใช้ Office อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="79379-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="79379-106">ปิดใช้งานแอปพลิเคชัน Windows Defender Guard (WDAG) หรือไฟร์วอลล์ที่คล้ายกันหรือโปรแกรมป้องกันไวรัส:</span><span class="sxs-lookup"><span data-stu-id="79379-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="79379-107">ในแผงควบคุมให้ไปที่**โปรแกรม**แล้วเลือก**เปิดหรือปิดฟีเจอร์ของ Windows**</span><span class="sxs-lookup"><span data-stu-id="79379-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="79379-108">ถ้าเปิดใช้งาน Guard ของแอปพลิเคชัน Windows Defender ให้ลองปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="79379-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="79379-109">**หมายเหตุ:** คุณอาจจำเป็นต้องเริ่มการทำงานของคอมพิวเตอร์ใหม่</span><span class="sxs-lookup"><span data-stu-id="79379-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="79379-110">ตรวจสอบให้แน่ใจว่า [ปลั๊กอิน BrokerPlugin AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ไม่ถูกบล็อกโดยแอปพลิเคชันหรือไฟร์วอลล์/โปรแกรมป้องกันไวรัส</span><span class="sxs-lookup"><span data-stu-id="79379-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="79379-111">[ล้างข้อมูลประจำตัวของ Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) โดยใช้ตัวจัดการข้อมูลประจำตัวของ Windows</span><span class="sxs-lookup"><span data-stu-id="79379-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="79379-112">**หมายเหตุ:** เส้นทางการลงทะเบียนของ Office 2016 เปลี่ยนเป็น 16.0 แล้ว</span><span class="sxs-lookup"><span data-stu-id="79379-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="79379-113">(เช่น: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="79379-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="79379-114">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ปัญหาการเชื่อมต่อในการลงชื่อเข้าใช้หลังจากอัปเดตเป็น Office ๒๐๑๖รุ่น16.0.7967 บน Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="79379-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>