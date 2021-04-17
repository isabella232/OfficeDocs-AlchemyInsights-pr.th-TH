---
title: การแก้ไขแอป Microsoft 365 ขออภัย เราอยู่ในข้อความปัญหาของเซิร์ฟเวอร์ชั่วคราว
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835290"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="7e5f2-102">การแก้ไขข้อความ "ขออภัย เราพบปัญหาเซิร์ฟเวอร์ชั่วคราว" ของแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7e5f2-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="7e5f2-103">ถ้าคุณได้รับข้อความนี้ ให้ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7e5f2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="7e5f2-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7e5f2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="7e5f2-105">ดู [URL และช่วงที่อยู่](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)IP</span><span class="sxs-lookup"><span data-stu-id="7e5f2-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="7e5f2-106">ไปที่ **เริ่ม**  >  **เรียกใช้** แล้วพิมพ์ **services.msc**</span><span class="sxs-lookup"><span data-stu-id="7e5f2-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="7e5f2-107">ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้ทั้งหมดถูกเรียกใช้อยู่:</span><span class="sxs-lookup"><span data-stu-id="7e5f2-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="7e5f2-108">การตั้งค่าอุปกรณ์ที่เชื่อมต่อเครือข่ายโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="7e5f2-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="7e5f2-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="7e5f2-109">Network List Service</span></span>
    - <span data-ttu-id="7e5f2-110">การรับรู้สถานที่ตั้งเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="7e5f2-110">Network Location Awareness</span></span>
    - <span data-ttu-id="7e5f2-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="7e5f2-111">Windows Event Log</span></span>

<span data-ttu-id="7e5f2-112">ถ้าหนึ่งในบริการเหล่านี้ไม่ได้เรียกใช้อยู่ ให้ลองเริ่มใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7e5f2-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="7e5f2-113">ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้สั่งต่อไปนี้โดยการเปิดพร้อมท์ของสั่งด้วยสิทธิ์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="7e5f2-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="7e5f2-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="7e5f2-114">**sfc /scannow**</span></span>

<span data-ttu-id="7e5f2-115">หลังจากเสร็จสิ้นการสั่งนี้ ให้รีสตาร์ตคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="7e5f2-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="7e5f2-116">ดูข้อมูลโดยละเอียดที่ ["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ ข้อผิดพลาด โปรดลองอีกครั้งในภายหลัง" เมื่อคุณ](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)เปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="7e5f2-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>