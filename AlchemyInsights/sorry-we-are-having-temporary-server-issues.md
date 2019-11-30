---
title: แก้ไขแอป Office ขออภัยเรากำลังมีข้อความแจ้งปัญหาเกี่ยวกับเซิร์ฟเวอร์แบบถาวร
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628009"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="d1941-102">แก้ไขแอป Office "ขออภัยเรากำลังมีปัญหาเซิร์ฟเวอร์การทำงานแบบถาวร" ข้อความ</span><span class="sxs-lookup"><span data-stu-id="d1941-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="d1941-103">ถ้าคุณได้รับข้อความนี้ให้ลองทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="d1941-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d1941-104">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office</span><span class="sxs-lookup"><span data-stu-id="d1941-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="d1941-105">ดู[url ของ Office ๓๖๕และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="d1941-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d1941-106">ไปที่**เริ่มต้น** > **รัน**และจากนั้นพิมพ์**บริการ. msc**</span><span class="sxs-lookup"><span data-stu-id="d1941-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d1941-107">ตรวจสอบให้แน่ใจว่าบริการต่อไปนี้ทั้งหมดทำงานอยู่:</span><span class="sxs-lookup"><span data-stu-id="d1941-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d1941-108">ตั้งค่าอุปกรณ์เชื่อมต่อเครือข่ายอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="d1941-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d1941-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="d1941-109">Network List Service</span></span>
    - <span data-ttu-id="d1941-110">การรับรู้ตำแหน่งเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="d1941-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d1941-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="d1941-111">Windows Event Log</span></span>

<span data-ttu-id="d1941-112">ถ้าหนึ่งในบริการเหล่านี้ไม่ได้ทำงานให้ลองเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="d1941-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d1941-113">ถ้าคุณมีปัญหาในการเริ่มต้นการบริการให้เรียกใช้คำสั่งต่อไปนี้โดยการเปิดพร้อมท์คำสั่งด้วยสิทธิ์ระดับสูง:</span><span class="sxs-lookup"><span data-stu-id="d1941-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d1941-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="d1941-114">**sfc /scannow**</span></span>

<span data-ttu-id="d1941-115">หลังจากคำสั่งนี้เสร็จสิ้นให้รีสตาร์ทเครื่องคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="d1941-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d1941-116">สำหรับข้อมูลรายละเอียดโปรดดู["ขออภัยเราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ กรุณาลองอีกครั้งในภายหลัง "ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office จาก Office ๓๖๕](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="d1941-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>