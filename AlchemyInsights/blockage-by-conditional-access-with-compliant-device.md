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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019167"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้ากันได้

**เครื่องมือที่แนะนาเป็นอย่างยิ่ง**

- [เครื่องมือแก้ไขปัญหาการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - เครื่องมือที่ครอบคลุมที่ช่วยแก้ไขปัญหาการลงทะเบียนอุปกรณ์ที่พบบ่อยที่สุด
- [ทดสอบสคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - เครื่องมือที่ใช้เพื่อให้แน่ใจว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบ
- [สคริปต์การล้างข้อมูลอุปกรณ์ Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - เครื่องมือที่ใช้ค้นหาและจัดการอุปกรณ์เก่าในสภาพแวดล้อมของคุณ

ต่อไปนี้เป็นสาเหตุทั่วไปบางประการที่ Access ตามเงื่อนไขอาจล้มเหลวในอุปกรณ์ที่เข้ากันได้ หรือสาเหตุที่ผู้ใช้ของคุณได้รับ คุณไม่สามารถรับจากข้อความที่นี่ระหว่างการร้องขอการลงชื่อเข้าใช้ไปยังทรัพยากรขององค์กร

1. **อุปกรณ์ไม่อยู่ในสถานะอุปกรณ์ที่ต้องมีกับ MDM**:

ตรวจสอบว่าอุปกรณ์ได้ลงทะเบียนกับผู้ให้บริการ MDM ที่ได้รับการอนุมัติแล้ว เช่น Intuned และถูก *ระบุว่าตรงตาม* มาตรฐาน ดูข้อมูลเพิ่มเติมเกี่ยวกับ Intun1 ดู [เอกสาร](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)นี้ เพื่อความเข้าใจเกี่ยวกับการปฏิบัติตามนโยบายอุปกรณ์และ Intun1 ที่ดียิ่งขึ้น ให้ดู[ใช้นโยบายการปฏิบัติตามนโยบายเพื่อตั้งค่ากฎของอุปกรณ์ที่คุณจัดการด้วย Intun1](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) ถ้าคุณมีปัญหาในการลงทะเบียนอุปกรณ์ด้วย Intuns ให้ค้นหารายละเอียดการแก้ไขปัญหา[ที่ แก้ไขปัญหาการลงทะเบียนอุปกรณ์ใน Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) สร้างการร้องขอการสนับสนุนเพื่อรับการสนับสนุนเพิ่มเติมจาก Intun1 หากต้องการเพิ่ม ให้ไปที่หน้า[บริการช่วยเหลือและวิธีใช้ Intuny](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **อุปกรณ์ไม่เชื่อมต่อกับเครือข่ายองค์กร**:

เพื่อให้สามารถเข้าถึงทรัพยากรขององค์กร อุปกรณ์ดังกล่าวจะต้องเชื่อมต่อกับเครือข่ายขององค์กร ผ่านการเชื่อมต่อโดยตรงหรือเครือข่ายส่วนตัวเสมือน (VPN) และเข้าร่วมในองค์กรหรือเครือข่ายAzure Active Directoryองค์กร เมื่อต้องการเข้าร่วมอุปกรณ์ที่ร่วมงานไปยังเครือข่าย [องค์กร ให้ดู เข้าร่วมอุปกรณ์ที่งานของคุณไปยังเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)องค์กรของคุณ เมื่อต้องการลงทะเบียนอุปกรณ์ส่วนบุคคล/BYOD ให้ดู [ลงทะเบียนอุปกรณ์ส่วนบุคคลของคุณบนเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)องค์กรของคุณ

- เมื่อต้องการตรวจสอบว่าอุปกรณ์ได้เข้าร่วมเครือข่ายหรือไม่ คุณสามารถปฏิบัติตามขั้นตอนของอุปกรณ์ที่ลงทะเบียน [ที่นี่](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) หรืออุปกรณ์ [ที่ได้ผล](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)ที่นี่ เมื่อต้องการขอบเขตปัญหาในการเชื่อมต่อเครือข่ายแบบ Org ให้ปฏิบัติตามแนวทางด้านล่าง:

    1. ลงชื่อเข้าใช้Windowsโดยใช้บัญชีที่โรงเรียนหรือที่ alain@contoso.com ของคุณ
    2. เชื่อมต่อเครือข่ายองค์กรของคุณผ่าน VPN หรือ DirectAccess
    3. หลังจากที่คุณเชื่อมต่อแล้ว ให้กดแป้นWindows **+L** เพื่อล็อกอุปกรณ์ของคุณ
    4. ปลดล็อกอุปกรณ์ของคุณโดยใช้บัญชีของที่โรงเรียนหรือที่โรงเรียน แล้วลองเข้าถึงแอปหรือบริการที่มีปัญหาอีกครั้ง

ถ้าคุณเห็น **ข้อความแสดงข้อผิดพลาด คุณไม่ได้รับจากที่นี่** อีกครั้ง ปัญหาอาจอยู่ที่อื่น

3. **ระบบปฏิบัติการไม่รองรับ**:

ตรวจสอบให้แน่ใจว่าคุณใช้ระบบปฏิบัติการรุ่นที่สนับสนุน ซึ่งรวมถึง:

- **Windowsไคลเอ็นต์**: Windows 7 หรือใหม่กว่า

- **Windows Server:** Windows Server 2008 R2 หรือใหม่กว่า

- **macOS**: macOS X หรือใหม่กว่า

- **Android และ iOS:** ระบบปฏิบัติการ Android และ iOS บนอุปกรณ์เคลื่อนที่เวอร์ชันล่าสุด

4. **เว็บเบราว์เซอร์ไม่ได้รับการสนับสนุน**:

โปรดค้นหาเบราว์เซอร์ที่สนับสนุนด้านล่าง For Chrome support with Windows 1703 or later versions, a Windows 10 accounts extension is required. For Edge 85+, the user needs to be signed in to properly pass device compliance information. หากต้องการรายละเอียดเพิ่มเติม [โปรดดู](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)ที่นี่

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS**: Microsoft Edge, เบราว์เซอร์ที่มีการจัดการ Intuned, Safari
- **Android**: **Microsoft Edge**: เบราว์เซอร์ที่มีการจัดการ Intuned, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

ค้นหาข้อมูลเพิ่มเติมเกี่ยวกับ **ข้อความที่คุณไม่สามารถรับได้ และ**[ขั้นตอนการแก้ไขปัญหาที่นี่](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
