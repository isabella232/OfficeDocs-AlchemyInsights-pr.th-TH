---
title: การแก้ไขแอป Microsoft 365 ขออภัยเรากําลังมีปัญหาเซิร์ฟเวอร์ชั่วคราว
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582722"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="4d416-102">การแก้ไขแอป Microsoft 365 "ขออภัยเรากําลังมีปัญหาเซิร์ฟเวอร์ชั่วคราว"</span><span class="sxs-lookup"><span data-stu-id="4d416-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="4d416-103">หากคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="4d416-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4d416-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4d416-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4d416-105">ดู[URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="4d416-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4d416-106">ไปที่**Start**  >  **เริ่มรัน**แล้วพิมพ์**services.msc**</span><span class="sxs-lookup"><span data-stu-id="4d416-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4d416-107">ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้ทั้งหมดทํางาน:</span><span class="sxs-lookup"><span data-stu-id="4d416-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4d416-108">อุปกรณ์เชื่อมต่อเครือข่ายอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="4d416-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4d416-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="4d416-109">Network List Service</span></span>
    - <span data-ttu-id="4d416-110">การรับรู้ตําแหน่งบนเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="4d416-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4d416-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="4d416-111">Windows Event Log</span></span>

<span data-ttu-id="4d416-112">หากบริการใดบริการหนึ่งเหล่านี้ไม่ทํางาน ให้ลองเริ่มต้นบริการดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="4d416-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4d416-113">ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้ โดยการเปิดพร้อมท์คําสั่งด้วยสิทธิ์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="4d416-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4d416-114">**/ สแกน**</span><span class="sxs-lookup"><span data-stu-id="4d416-114">**sfc /scannow**</span></span>

<span data-ttu-id="4d416-115">หลังจากคําสั่งนี้เสร็จสิ้น แล้ว ให้รีสตาร์ทคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="4d416-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4d416-116">สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="4d416-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>