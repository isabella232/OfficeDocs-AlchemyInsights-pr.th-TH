---
title: การแก้ไขแอป Office Sorry เรากําลังมีข้อความเกี่ยวกับปัญหาเซิร์ฟเวอร์ชั่วคราว
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764136"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="5d1da-102">การแก้ไขแอป Office "ขออภัย เรากําลังมีปัญหาชั่วคราวของเซิร์ฟเวอร์"</span><span class="sxs-lookup"><span data-stu-id="5d1da-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="5d1da-103">ถ้าคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="5d1da-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="5d1da-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าจะไม่บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office</span><span class="sxs-lookup"><span data-stu-id="5d1da-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="5d1da-105">ดู[URL และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="5d1da-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="5d1da-106">ไปที่**เริ่ม** > **เรียกใช้**แล้วพิมพ์**services.msc**</span><span class="sxs-lookup"><span data-stu-id="5d1da-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="5d1da-107">ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้กําลังทํางานอยู่ทั้งหมด:</span><span class="sxs-lookup"><span data-stu-id="5d1da-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="5d1da-108">อุปกรณ์ที่เชื่อมต่อเครือข่ายอัตโนมัติติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="5d1da-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="5d1da-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="5d1da-109">Network List Service</span></span>
    - <span data-ttu-id="5d1da-110">การรับรู้ตําแหน่งบนเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="5d1da-110">Network Location Awareness</span></span>
    - <span data-ttu-id="5d1da-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="5d1da-111">Windows Event Log</span></span>

<span data-ttu-id="5d1da-112">ถ้าบริการเหล่านี้ไม่ได้ทํางานอยู่ ให้ลองเริ่มการทํางาน</span><span class="sxs-lookup"><span data-stu-id="5d1da-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="5d1da-113">ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้โดยการเปิดพร้อมท์คําสั่งที่มีสิทธิ์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="5d1da-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="5d1da-114">**sfc /สแกนโนว**</span><span class="sxs-lookup"><span data-stu-id="5d1da-114">**sfc /scannow**</span></span>

<span data-ttu-id="5d1da-115">หลังจากคําสั่งนี้เสร็จสิ้น ให้รีสตาร์ทคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="5d1da-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="5d1da-116">สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"ข้อผิดพลาดเมื่อคุณเปิดใช้งาน](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="5d1da-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>