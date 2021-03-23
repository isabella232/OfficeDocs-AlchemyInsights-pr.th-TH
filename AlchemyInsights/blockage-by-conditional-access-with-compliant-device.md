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
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้ากันได้

**เครื่องมือที่แนะนาเป็นอย่างยิ่ง**

- [เครื่องมือแก้ไขปัญหาการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - เครื่องมือที่ครอบคลุมซึ่งจะช่วยแก้ไขปัญหาการลงทะเบียนอุปกรณ์ที่พบบ่อยที่สุด
- [ทดสอบสคริปต์การเชื่อมต่อการลงทะเบียน](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) อุปกรณ์ - เครื่องมือที่ใช้เพื่อให้แน่ใจว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบ
- [สคริปต์การล้างข้อมูลอุปกรณ์ Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - เครื่องมือที่ใช้ค้นหาและจัดการอุปกรณ์เก่าในสภาพแวดล้อมของคุณ

ต่อไปนี้คือสาเหตุทั่วไปว่าเหตุใดการเข้าถึงตามเงื่อนไขอาจล้มเหลวบนอุปกรณ์ที่เข้ากันได้ หรือเหตุใดผู้ใช้ของคุณจึงได้รับข้อความจากที่นี่ในระหว่างการร้องขอการลงชื่อเข้าใช้ไปยังทรัพยากรขององค์กร

1. **อุปกรณ์ไม่อยู่ในสถานะอุปกรณ์ที่ต้องมีกับ MDM:**

ตรวจสอบว่าอุปกรณ์ได้รับการลงทะเบียนกับผู้ให้บริการ MDM ที่ได้รับอนุมัติ เช่น Intun>และมีการ *เครื่องหมายเป็นปฏิบัติตาม* นโยบายแล้ว หากต้องการข้อมูลเพิ่มเติมเกี่ยวกับ Intun1 ให้ดู [เอกสาร](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)นี้ เพื่อให้เข้าใจการปฏิบัติตามนโยบายของอุปกรณ์และ Intun1 ที่ดียิ่งขึ้น ให้ดูนโยบายการปฏิบัติตาม[นโยบายเพื่อตั้งค่ากฎบนอุปกรณ์ที่คุณจัดการด้วย Intun1](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) ถ้าคุณมีปัญหาในการลงทะเบียนอุปกรณ์ด้วย Intun1 ให้ค้นหารายละเอียดการแก้ไขปัญหา[ที่ แก้ไขปัญหาการลงทะเบียนอุปกรณ์ใน Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) หากต้องการรับการสนับสนุนเพิ่มเติม ให้สร้างการร้องขอการสนับสนุน เมื่อต้องการเลือก ให้ไปที่หน้า[ความช่วยเหลือและการสนับสนุน Intun1](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **อุปกรณ์ไม่เชื่อมต่อกับเครือข่ายขององค์กร**:

เพื่อการเข้าถึงทรัพยากรขององค์กร อุปกรณ์จะต้องเชื่อมต่อกับเครือข่ายขององค์กรผ่านการเชื่อมต่อโดยตรงหรือเครือข่ายส่วนตัวเสมือน (VPN) และเข้าร่วมในองค์กรหรือ Azure Active Directory เมื่อต้องการเข้าร่วมอุปกรณ์ที่ร่วมงานกับเครือข่ายองค์กร [ให้ดู เข้าร่วมอุปกรณ์ที่งานของคุณไปยังเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)องค์กรของคุณ เมื่อต้องการลงทะเบียนอุปกรณ์ส่วนบุคคล/BYOD ให้ดู ลงทะเบียน [อุปกรณ์ส่วนบุคคลของคุณบนเครือข่ายของ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)องค์กรของคุณ

- เมื่อต้องการตรวจสอบว่าอุปกรณ์ได้เข้าร่วมเครือข่ายแล้วหรือไม่ คุณสามารถปฏิบัติตามขั้นตอนของอุปกรณ์ที่ลงทะเบียน [ที่นี่](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) หรือ [อุปกรณ์ที่ร่วมงาน](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)ได้ที่นี่ เมื่อต้องการขอบเขตปัญหาในการเชื่อมต่อเครือข่ายแบบ Org ให้ปฏิบัติตามแนวทางด้านล่าง:

    1. ลงชื่อเข้าใช้ Windows โดยใช้บัญชีที่โรงเรียนหรือที่ alain@contoso.com ของคุณ
    2. เชื่อมต่อกับเครือข่ายขององค์กรของคุณผ่าน VPN หรือ DirectAccess
    3. หลังจากเชื่อมต่อแล้ว ให้กดแป้นโลโก้ **Windows+L** เพื่อล็อกอุปกรณ์ของคุณ
    4. ปลดล็อกอุปกรณ์ของคุณโดยใช้บัญชีที่โรงเรียนหรือที่โรงเรียนแล้วลองเข้าถึงแอปหรือบริการที่มีปัญหาอีกครั้ง

ถ้าคุณเห็น **ข้อความแสดงข้อผิดพลาด คุณไม่สามารถได้จากที่นี่** อีก ปัญหาอาจอยู่ที่อื่น

3. **ระบบปฏิบัติการไม่ได้รับการสนับสนุน**:

ตรวจสอบให้แน่ใจว่าคุณใช้งานระบบปฏิบัติการรุ่นที่สนับสนุน รวมถึง:

- **Windows Client**: Windows 7 หรือใหม่กว่า

- **Windows Server**: Windows Server 2008 R2 หรือใหม่กว่า

- **macOS**: macOS X หรือใหม่กว่า

- **Android และ iOS:** ระบบปฏิบัติการ Android และ iOS บนอุปกรณ์เคลื่อนที่เวอร์ชันล่าสุด

4. **เว็บเบราว์เซอร์ไม่ได้รับการสนับสนุน**:

โปรดค้นหาเบราว์เซอร์ที่รองรับด้านล่าง ต้องมีส่วนขยายบัญชี Windows 10 เพื่อรับการสนับสนุนเกี่ยวกับ Chrome ด้วย Windows 1703 หรือเวอร์ชันที่ใหม่กว่า For Edge 85+, the user needs be signed in to properly pass device compliance information. โปรดดูรายละเอียดเพิ่มเติม[ที่นี่](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, เบราว์เซอร์ที่มีการจัดการ Intuned, Safari
- **Android**: **Microsoft Edge**: เบราว์เซอร์ Intuned ที่มีการจัดการ, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

ค้นหาข้อมูลเพิ่มเติมเกี่ยวกับขั้นตอนที่ **คุณไม่สามารถรับข้อความและ** ขั้นตอนการแก้ไขปัญหา [ได้ที่นี่](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
