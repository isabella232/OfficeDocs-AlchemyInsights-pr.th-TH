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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716191"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="531ff-102">การแก้ไขแอป Office "เราไม่สามารถเชื่อมต่อได้ในขณะนี้"</span><span class="sxs-lookup"><span data-stu-id="531ff-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="531ff-103">ถ้าคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="531ff-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="531ff-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าจะไม่บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office</span><span class="sxs-lookup"><span data-stu-id="531ff-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="531ff-105">ดู[URL ของ Microsoft และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="531ff-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="531ff-106">ไปที่**เริ่ม** > **เรียกใช้**แล้วพิมพ์**services.msc**</span><span class="sxs-lookup"><span data-stu-id="531ff-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="531ff-107">ตรวจสอบให้แน่ใจว่า บริการต่อไปนี้กําลังทํางานอยู่ทั้งหมด:</span><span class="sxs-lookup"><span data-stu-id="531ff-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="531ff-108">อุปกรณ์ที่เชื่อมต่อเครือข่ายอัตโนมัติติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="531ff-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="531ff-109">บริการรายการเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="531ff-109">Network List Service</span></span>
    - <span data-ttu-id="531ff-110">การรับรู้ตําแหน่งบนเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="531ff-110">Network Location Awareness</span></span>
    - <span data-ttu-id="531ff-111">แฟ้มบันทึกเหตุการณ์ของ Windows</span><span class="sxs-lookup"><span data-stu-id="531ff-111">Windows Event Log</span></span>

<span data-ttu-id="531ff-112">ถ้าบริการเหล่านี้ไม่ได้ทํางานอยู่ ให้ลองเริ่มการทํางาน</span><span class="sxs-lookup"><span data-stu-id="531ff-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="531ff-113">ถ้าคุณมีปัญหาในการเริ่มบริการ ให้เรียกใช้คําสั่งต่อไปนี้โดยการเปิดพร้อมท์คําสั่งที่มีสิทธิ์ผู้ดูแล:</span><span class="sxs-lookup"><span data-stu-id="531ff-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="531ff-114">**sfc /สแกนโนว**</span><span class="sxs-lookup"><span data-stu-id="531ff-114">**sfc /scannow**</span></span>

<span data-ttu-id="531ff-115">หลังจากคําสั่งนี้เสร็จสิ้น ให้รีสตาร์ทคอมพิวเตอร์</span><span class="sxs-lookup"><span data-stu-id="531ff-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="531ff-116">สําหรับข้อมูลโดยละเอียด โปรดดูที่["ขออภัย เราไม่สามารถเชื่อมต่อกับบัญชีของคุณได้ โปรดลองอีกครั้งในภายหลัง"ข้อผิดพลาดเมื่อคุณเปิดใช้งาน Office จาก Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="531ff-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>