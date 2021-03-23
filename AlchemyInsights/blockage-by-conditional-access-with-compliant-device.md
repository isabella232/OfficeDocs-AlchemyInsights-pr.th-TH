---
title: ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้ากันได้
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037079"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="b8fb1-102">ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้ากันได้</span><span class="sxs-lookup"><span data-stu-id="b8fb1-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="b8fb1-103">**เครื่องมือที่แนะนาเป็นอย่างยิ่ง**</span><span class="sxs-lookup"><span data-stu-id="b8fb1-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="b8fb1-104">[เครื่องมือแก้ไขปัญหาการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - เครื่องมือที่ครอบคลุมซึ่งจะช่วยแก้ไขปัญหาการลงทะเบียนอุปกรณ์ที่พบบ่อยที่สุด</span><span class="sxs-lookup"><span data-stu-id="b8fb1-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="b8fb1-105">[ทดสอบสคริปต์การเชื่อมต่อการลงทะเบียน](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) อุปกรณ์ - เครื่องมือที่ใช้เพื่อให้แน่ใจว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบ</span><span class="sxs-lookup"><span data-stu-id="b8fb1-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="b8fb1-106">[สคริปต์การล้างข้อมูลอุปกรณ์ Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - เครื่องมือที่ใช้ค้นหาและจัดการอุปกรณ์เก่าในสภาพแวดล้อมของคุณ</span><span class="sxs-lookup"><span data-stu-id="b8fb1-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="b8fb1-107">ต่อไปนี้คือสาเหตุทั่วไปว่าเหตุใดการเข้าถึงตามเงื่อนไขอาจล้มเหลวบนอุปกรณ์ที่เข้ากันได้ หรือเหตุใดผู้ใช้ของคุณจึงได้รับข้อความจากที่นี่ในระหว่างการร้องขอการลงชื่อเข้าใช้ไปยังทรัพยากรขององค์กร</span><span class="sxs-lookup"><span data-stu-id="b8fb1-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="b8fb1-108">**อุปกรณ์ไม่อยู่ในสถานะอุปกรณ์ที่ต้องมีกับ MDM:**</span><span class="sxs-lookup"><span data-stu-id="b8fb1-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="b8fb1-109">ตรวจสอบว่าอุปกรณ์ได้รับการลงทะเบียนกับผู้ให้บริการ MDM ที่ได้รับอนุมัติ เช่น Intun>และมีการ *เครื่องหมายเป็นปฏิบัติตาม* นโยบายแล้ว</span><span class="sxs-lookup"><span data-stu-id="b8fb1-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="b8fb1-110">หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับ Intun1 ให้ดู [เอกสาร](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)นี้</span><span class="sxs-lookup"><span data-stu-id="b8fb1-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="b8fb1-111">เพื่อให้เข้าใจการปฏิบัติตามนโยบายของอุปกรณ์และ Intun1 ที่ดียิ่งขึ้น ให้ดูนโยบายการปฏิบัติตาม[นโยบายเพื่อตั้งค่ากฎบนอุปกรณ์ที่คุณจัดการด้วย Intun1](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="b8fb1-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="b8fb1-112">ถ้าคุณมีปัญหาในการลงทะเบียนอุปกรณ์ด้วย Intun1 ให้ค้นหารายละเอียดการแก้ไขปัญหา[ที่ แก้ไขปัญหาการลงทะเบียนอุปกรณ์ใน Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="b8fb1-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="b8fb1-113">หากต้องการรับการสนับสนุนเพิ่มเติม ให้สร้างการร้องขอการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="b8fb1-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="b8fb1-114">เมื่อต้องการเลือก ให้ไปที่หน้า[ความช่วยเหลือและการสนับสนุน Intun1](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)</span><span class="sxs-lookup"><span data-stu-id="b8fb1-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="b8fb1-115">**อุปกรณ์ไม่เชื่อมต่อกับเครือข่ายขององค์กร**:</span><span class="sxs-lookup"><span data-stu-id="b8fb1-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="b8fb1-116">เพื่อการเข้าถึงทรัพยากรขององค์กร อุปกรณ์จะต้องเชื่อมต่อกับเครือข่ายขององค์กรผ่านการเชื่อมต่อโดยตรงหรือเครือข่ายส่วนตัวเสมือน (VPN) และเข้าร่วมในองค์กรหรือ Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b8fb1-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="b8fb1-117">เมื่อต้องการเข้าร่วมอุปกรณ์ที่ร่วมงานกับเครือข่ายองค์กร [ให้ดู เข้าร่วมอุปกรณ์ที่งานของคุณไปยังเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)องค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b8fb1-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="b8fb1-118">เมื่อต้องการลงทะเบียนอุปกรณ์ส่วนบุคคล/BYOD ให้ดู ลงทะเบียน [อุปกรณ์ส่วนบุคคลของคุณบนเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)องค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="b8fb1-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="b8fb1-119">เมื่อต้องการตรวจสอบว่าอุปกรณ์ได้เข้าร่วมเครือข่ายแล้วหรือไม่ คุณสามารถปฏิบัติตามขั้นตอนของอุปกรณ์ที่ลงทะเบียน [ที่นี่](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) หรือ [อุปกรณ์ที่ร่วมงาน](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)ได้ที่นี่</span><span class="sxs-lookup"><span data-stu-id="b8fb1-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="b8fb1-120">เมื่อต้องการขอบเขตปัญหาในการเชื่อมต่อเครือข่ายแบบ Org ให้ปฏิบัติตามแนวทางด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="b8fb1-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="b8fb1-121">ลงชื่อเข้าใช้ Windows โดยใช้บัญชีที่โรงเรียนหรือที่ alain@contoso.com ของคุณ</span><span class="sxs-lookup"><span data-stu-id="b8fb1-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="b8fb1-122">เชื่อมต่อกับเครือข่ายขององค์กรของคุณผ่าน VPN หรือ DirectAccess</span><span class="sxs-lookup"><span data-stu-id="b8fb1-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="b8fb1-123">หลังจากเชื่อมต่อแล้ว ให้กดแป้นโลโก้ **Windows+L** เพื่อล็อกอุปกรณ์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="b8fb1-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="b8fb1-124">ปลดล็อกอุปกรณ์ของคุณโดยใช้บัญชีที่โรงเรียนหรือที่โรงเรียนแล้วลองเข้าถึงแอปหรือบริการที่มีปัญหาอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="b8fb1-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="b8fb1-125">ถ้าคุณเห็น **ข้อความแสดงข้อผิดพลาด คุณไม่สามารถได้จากที่นี่** อีก ปัญหาอาจอยู่ที่อื่น</span><span class="sxs-lookup"><span data-stu-id="b8fb1-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="b8fb1-126">**ระบบปฏิบัติการไม่ได้รับการสนับสนุน**:</span><span class="sxs-lookup"><span data-stu-id="b8fb1-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="b8fb1-127">ตรวจสอบให้แน่ใจว่าคุณใช้งานระบบปฏิบัติการรุ่นที่สนับสนุน รวมถึง:</span><span class="sxs-lookup"><span data-stu-id="b8fb1-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="b8fb1-128">**Windows Client**: Windows 7 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="b8fb1-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="b8fb1-129">**Windows Server**: Windows Server 2008 R2 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="b8fb1-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="b8fb1-130">**macOS**: macOS X หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="b8fb1-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="b8fb1-131">**Android และ iOS:** ระบบปฏิบัติการ Android และ iOS บนอุปกรณ์เคลื่อนที่เวอร์ชันล่าสุด</span><span class="sxs-lookup"><span data-stu-id="b8fb1-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="b8fb1-132">**เว็บเบราว์เซอร์ไม่ได้รับการสนับสนุน**:</span><span class="sxs-lookup"><span data-stu-id="b8fb1-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="b8fb1-133">โปรดค้นหาเบราว์เซอร์ที่รองรับด้านล่าง</span><span class="sxs-lookup"><span data-stu-id="b8fb1-133">Please find supported browsers below.</span></span> <span data-ttu-id="b8fb1-134">ต้องมีส่วนขยายบัญชี Windows 10 เพื่อรับการสนับสนุนเกี่ยวกับ Chrome ด้วย Windows 1703 หรือเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="b8fb1-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="b8fb1-135">For Edge 85+, the user needs be signed in to properly pass device compliance information.</span><span class="sxs-lookup"><span data-stu-id="b8fb1-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="b8fb1-136">โปรดดูรายละเอียดเพิ่มเติม[ที่นี่](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="b8fb1-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="b8fb1-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="b8fb1-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b8fb1-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="b8fb1-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b8fb1-139">**Windows 7**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="b8fb1-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b8fb1-140">**iOS**: Microsoft Edge, เบราว์เซอร์ที่มีการจัดการ Intuned, Safari</span><span class="sxs-lookup"><span data-stu-id="b8fb1-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="b8fb1-141">**Android**: **Microsoft Edge**: เบราว์เซอร์ Intuned ที่มีการจัดการ, Chrome</span><span class="sxs-lookup"><span data-stu-id="b8fb1-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="b8fb1-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b8fb1-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="b8fb1-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="b8fb1-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b8fb1-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b8fb1-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="b8fb1-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b8fb1-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="b8fb1-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b8fb1-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="b8fb1-147">**macOS**: Chrome, Safari</span><span class="sxs-lookup"><span data-stu-id="b8fb1-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="b8fb1-148">ค้นหาข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนที่ **คุณไม่สามารถรับข้อความและ** ขั้นตอนการแก้ไขปัญหา [ได้ที่นี่](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)</span><span class="sxs-lookup"><span data-stu-id="b8fb1-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
