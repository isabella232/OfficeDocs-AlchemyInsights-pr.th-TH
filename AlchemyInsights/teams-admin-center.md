---
title: ศูนย์การจัดการทีม
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670383"
---
# <a name="teams-admin-center"></a><span data-ttu-id="51b2c-102">ศูนย์การจัดการทีม</span><span class="sxs-lookup"><span data-stu-id="51b2c-102">Teams Admin Center</span></span>

<span data-ttu-id="51b2c-103">เรียนรู้เกี่ยวกับการจัดการทีมด้วย[ศูนย์การจัดการทีม](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)</span><span class="sxs-lookup"><span data-stu-id="51b2c-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="51b2c-104">ถ้าคุณไม่สามารถเข้าถึงศูนย์การจัดการทีมโปรดตรวจสอบรายการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="51b2c-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="51b2c-105">ตรวจสอบว่าคุณได้อนุญาตให้ใช้ที่ [อยู่ IP ของ Office ๓๖๕](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) ที่เหมาะสมและ URL บนอุปกรณ์ขอบเขตใดก็ได้ (ไฟร์วอลล์ฯลฯ) หรือในกฎไฟร์วอลล์บนเครื่องคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="51b2c-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="51b2c-106">ตรวจสอบว่าการเข้าสู่ระบบที่คุณใช้ในการเข้าถึงพอร์ทัลผู้ดูแลระบบของทีมตรงกับชื่อผู้ใช้ของคุณที่แสดงรายการอยู่ใน[พอร์ทัลผู้ดูแลระบบ Microsoft ๓๖๕](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="51b2c-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="51b2c-107">ถ้าผู้ใช้ไม่ปรากฏในศูนย์การจัดการทีมโปรดตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="51b2c-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="51b2c-108">คุณสร้างผู้ใช้หรือสิทธิ์การใช้งานที่มอบหมายใน24ชั่วโมงที่ผ่านมาหรือไม่</span><span class="sxs-lookup"><span data-stu-id="51b2c-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="51b2c-109">โปรดตรวจสอบให้แน่ใจว่าคุณรออย่างน้อย24ชั่วโมงก่อนที่จะเปิดบัตรสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="51b2c-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="51b2c-110">ตรวจสอบว่าคุณได้กำหนดสิทธิ์การใช้งานที่เหมาะสมแล้วหรือยัง</span><span class="sxs-lookup"><span data-stu-id="51b2c-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="51b2c-111">ถ้าคุณมีไดเรกทอรีที่ใช้งานอยู่ภายในองค์กรให้ตรวจสอบว่า[ค่าของ msRTCSIP-PrimaryUserAddress หรือที่อยู่ SIP ในเขตข้อมูล ProxyAddresses ใน Active directory ภายในเครื่องของคุณจะไม่ซ้ำกันและรูปแบบที่ตรงกับ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)SIP:**ชื่อ**ผู้ใช้ของผู้ใช้จาก[ศูนย์การจัดการ Microsoft ๓๖๕](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="51b2c-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="51b2c-112">ถ้าคุณต้องการเก็บการปรับใช้ Skype for Business Server และมีผู้ใช้ที่ homed ภายในองค์กรและออนไลน์: ให้ทำตามขั้นตอน **"ตั้งค่าไฮบริดที่มีทีมและ skype For Business Online"** ในแผงควบคุมเซิร์ฟเวอร์ Skype for business ของคุณและย้ายผู้ใช้แบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="51b2c-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
