---
title: ศูนย์การจัดการทีม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354107"
---
# <a name="teams-admin-center"></a><span data-ttu-id="38b89-102">ศูนย์การจัดการทีม</span><span class="sxs-lookup"><span data-stu-id="38b89-102">Teams Admin Center</span></span>

<span data-ttu-id="38b89-103">เรียนรู้เกี่ยวกับการจัดการทีมด้วย[ศูนย์การจัดการทีม](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)</span><span class="sxs-lookup"><span data-stu-id="38b89-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="38b89-104">หากคุณไม่สามารถเข้าถึงศูนย์การจัดการทีม โปรดตรวจสอบรายการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="38b89-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="38b89-105">ตรวจสอบว่า คุณได้รับอนุญาต[ที่เหมาะสมอยู่ IP 365 Office และ URL ใน](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)อุปกรณ์ในขอบเขตใด ๆ (ไฟร์วอลล์ ฯลฯ ) หรือในกฎไฟร์วอลล์บนเครื่องของคุณ</span><span class="sxs-lookup"><span data-stu-id="38b89-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="38b89-106">ตรวจสอบว่าล็อกอินที่คุณใช้ในการเข้าถึงพอร์ทัล Admin Teams ตรงกับชื่อผู้ใช้ของคุณที่แสดงรายการอยู่ใน[พอร์ทัลการดูแลระบบของ Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="38b89-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="38b89-107">ถ้าผู้ใช้ไม่ปรากฏในศูนย์การจัดการทีม โปรดตรวจสอบดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="38b89-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="38b89-108">คุณได้สร้างผู้ใช้หรือสิทธิ์การใช้งานที่ได้รับมอบหมายในช่วง 24 ชั่วโมงที่ผ่านมาหรือไม่</span><span class="sxs-lookup"><span data-stu-id="38b89-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="38b89-109">โปรดรออย่างน้อย 24 ชั่วโมงก่อนเปิดตั๋วสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="38b89-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="38b89-110">ตรวจสอบว่าคุณได้กําหนดสิทธิ์การใช้งานที่เหมาะสมแล้วหรือไม่</span><span class="sxs-lookup"><span data-stu-id="38b89-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="38b89-111">ถ้าคุณมีไดเรกทอรีที่ใช้งานอยู่ในสถานที่ ตรวจสอบว่า[ค่าของ msRTCSIP PrimaryUserAddress หรืออยู่ SIP ในเขตข้อมูล ProxyAddresses ในไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องของคุณไม่ซ้ํากัน และรูปแบบที่ตรงกับ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)จิบ:**ชื่อผู้ใช้**จาก[ศูนย์การจัดการ Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="38b89-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="38b89-112">ถ้าคุณตั้งใจจะเก็บ Skype สําหรับการปรับใช้เซิร์ฟเวอร์ธุรกิจ และมีผู้ใช้ homed ในสถาน และออนไลน์: ทําตาม **"ตั้งค่าไฮบริดสลี กับทีมและ Skype สําหรับธุรกิจออนไลน์"** ใน Skype ของคุณสําหรับแผงควบคุมเซิร์ฟเวอร์ธุรกิจ และย้ายผู้ใช้แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="38b89-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
