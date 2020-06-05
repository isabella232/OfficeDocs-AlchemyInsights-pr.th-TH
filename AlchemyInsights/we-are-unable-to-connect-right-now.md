---
title: ปัญหาการเปิดใช้งาน - เราไม่สามารถเชื่อมต่อได้ในขณะนี้
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581894"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="dae98-102">การแก้ไขแอป Microsoft 365 "เราไม่สามารถเชื่อมต่อได้ในขณะนี้" ข้อความ</span><span class="sxs-lookup"><span data-stu-id="dae98-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="dae98-103">หากคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="dae98-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="dae98-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="dae98-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="dae98-105">ดู[URL ของ Microsoft และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="dae98-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="dae98-106">ไปที่**Start**  >  **เริ่มรัน**แล้วพิมพ์**services.msc**</span><span class="sxs-lookup"><span data-stu-id="dae98-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="dae98-107">ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้ทั้งหมดทํางาน:</span><span class="sxs-lookup"><span data-stu-id="dae98-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="dae98-108">อุปกรณ์เชื่อมต่อเครือข่ายอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="dae98-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="dae98-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="dae98-109">Network List Service</span></span>
    - <span data-ttu-id="dae98-110">การรับรู้ตําแหน่งบนเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="dae98-110">Network Location Awareness</span></span>
    - <span data-ttu-id="dae98-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="dae98-111">Windows Event Log</span></span>

<span data-ttu-id="dae98-112">หากบริการใดบริการหนึ่งเหล่านี้ไม่ทํางาน ให้ลองเริ่มต้นบริการดังกล่าว</span><span class="sxs-lookup"><span data-stu-id="dae98-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="dae98-113">ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้ โดยการเปิดพร้อมท์คําสั่งด้วยสิทธิ์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="dae98-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="dae98-114">**/ สแกน**</span><span class="sxs-lookup"><span data-stu-id="dae98-114">**sfc /scannow**</span></span>

<span data-ttu-id="dae98-115">หลังจากคําสั่งนี้เสร็จสิ้น แล้ว ให้รีสตาร์ทคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="dae98-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="dae98-116">สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="dae98-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>