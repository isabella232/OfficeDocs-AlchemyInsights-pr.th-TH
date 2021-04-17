---
title: ศูนย์การจัดการ Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826398"
---
# <a name="teams-admin-center"></a><span data-ttu-id="7c435-102">ศูนย์การจัดการ Teams</span><span class="sxs-lookup"><span data-stu-id="7c435-102">Teams Admin Center</span></span>

<span data-ttu-id="7c435-103">เรียนรู้เกี่ยวกับการจัดการ Teams ด้วย [ศูนย์การจัดการ](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)Teams</span><span class="sxs-lookup"><span data-stu-id="7c435-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="7c435-104">ถ้าคุณไม่สามารถเข้าถึงศูนย์การจัดการ Teams โปรดตรวจสอบรายการต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7c435-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="7c435-105">ตรวจสอบว่าคุณได้อนุญาตที่อยู่ [IP และ URL ของ Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) ที่เหมาะสมบนอุปกรณ์เฉพาะเขตใดๆ (ไฟร์วอลล์ และอื่นๆ) หรือในกฎไฟร์วอลล์บนเครื่องคอมพิวเตอร์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="7c435-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="7c435-106">ตรวจสอบว่าการเข้าสู่ระบบที่คุณใช้เพื่อเข้าถึงพอร์ทัลการดูแลระบบ Teams ตรงกับชื่อผู้ใช้ของคุณที่แสดงในพอร์ทัล[ผู้ดูแลระบบ Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="7c435-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="7c435-107">ถ้าผู้ใช้ไม่ปรากฏในศูนย์การจัดการ Teams โปรดตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7c435-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="7c435-108">คุณได้สร้างผู้ใช้หรือสิทธิ์การใช้งานที่ได้รับมอบหมายใน 24 ชั่วโมงที่ผ่านมาแล้วหรือยัง</span><span class="sxs-lookup"><span data-stu-id="7c435-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="7c435-109">โปรดตรวจสอบให้แน่ใจว่าคุณรออย่างน้อย 24 ชั่วโมงก่อนที่จะเปิดตั๋วการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="7c435-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="7c435-110">ตรวจสอบว่าคุณได้มอบหมายสิทธิ์การใช้งานที่เหมาะสมหรือไม่</span><span class="sxs-lookup"><span data-stu-id="7c435-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="7c435-111">ถ้าคุณมี Active Directory ภายในองค์กร ให้ตรวจสอบว่าค่าของ [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)หรือที่อยู่ SIP ในเขตข้อมูล ProxyAddresses ใน Active Directory ภายในเครื่องของคุณไม่ซ้ิอกัน และรูปแบบตรงกับ **sip:** ชื่อผู้ใช้ของผู้ใช้จากศูนย์การจัดการ [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="7c435-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="7c435-112">ถ้าคุณต้องการเก็บการปรับใช้ Skype for Business Server และให้ผู้ใช้อยู่ในองค์กรและออนไลน์: ติดตาม "ตั้งค่าแบบไฮบริดกับ Teams และ **Skype for Business Online"** ในแผงควบคุม Skype for Business Server ของคุณ และย้ายผู้ใช้ออนไลน์</span><span class="sxs-lookup"><span data-stu-id="7c435-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
