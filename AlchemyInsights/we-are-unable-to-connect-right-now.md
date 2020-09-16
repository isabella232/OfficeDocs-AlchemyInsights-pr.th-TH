---
title: ปัญหาการเปิดใช้งาน-เราไม่สามารถเชื่อมต่อได้ในขณะนี้
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726002"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="acd98-102">การแก้ไขแอป Microsoft ๓๖๕ "เราไม่สามารถเชื่อมต่อได้ในขณะนี้" ข้อความ</span><span class="sxs-lookup"><span data-stu-id="acd98-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="acd98-103">ถ้าคุณได้รับข้อความนี้ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="acd98-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="acd98-104">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="acd98-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="acd98-105">ให้ดู[ที่ url และช่วงที่อยู่ IP ของ Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="acd98-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="acd98-106">ไปที่**เริ่ม**  >  **เรียกใช้**แล้วพิมพ์**msc**</span><span class="sxs-lookup"><span data-stu-id="acd98-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="acd98-107">ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้กำลังทำงานอยู่ทั้งหมด:</span><span class="sxs-lookup"><span data-stu-id="acd98-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="acd98-108">การตั้งค่าอุปกรณ์ที่เชื่อมต่อเครือข่ายโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="acd98-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="acd98-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="acd98-109">Network List Service</span></span>
    - <span data-ttu-id="acd98-110">การรับรู้ตำแหน่งบนเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="acd98-110">Network Location Awareness</span></span>
    - <span data-ttu-id="acd98-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="acd98-111">Windows Event Log</span></span>

<span data-ttu-id="acd98-112">ถ้าหนึ่งในบริการเหล่านี้ไม่ได้ทำงานอยู่ให้ลองเริ่มต้นใช้งาน</span><span class="sxs-lookup"><span data-stu-id="acd98-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="acd98-113">ถ้าคุณมีปัญหาในการเริ่มบริการให้เรียกใช้คำสั่งต่อไปนี้โดยการเปิดพร้อมท์คำสั่งด้วยสิทธิ์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="acd98-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="acd98-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="acd98-114">**sfc /scannow**</span></span>

<span data-ttu-id="acd98-115">หลังจากคำสั่งนี้เสร็จสิ้นให้รีสตาร์ตเครื่องคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="acd98-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="acd98-116">สำหรับข้อมูลโดยละเอียดให้ดู[ที่ "ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีผู้ใช้ของคุณได้ โปรดลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office จาก Microsoft ๓๖๕](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="acd98-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>