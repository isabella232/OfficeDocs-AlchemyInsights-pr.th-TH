---
title: ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้าร่วมในโดเมน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038105"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้าร่วมในโดเมน

**เครื่องมือที่แนะนาเป็นอย่างยิ่ง**

[เครื่องมือแก้ไขปัญหาการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - เครื่องมือที่จะช่วยแก้ไขปัญหาการลงทะเบียนอุปกรณ์ที่พบบ่อยที่สุด

[ทดสอบสคริปต์การเชื่อมต่อการลงทะเบียน](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) อุปกรณ์ - สคริปต์ที่ช่วยรับรองว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบ

[สคริปต์การล้างข้อมูลอุปกรณ์ Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - สคริปต์ที่ช่วยให้คุณค้นหาและจัดการอุปกรณ์เก่าในสภาพแวดล้อมของคุณ

ต่อไปนี้เป็นสาเหตุทั่วไปบางประการที่การเข้าถึงตามเงื่อนไขอาจล้มเหลวอุปกรณ์ที่เข้าร่วมโดเมน (Hybrid Azure AD)

1. **ไม่มี Azure AD PRT บนอุปกรณ์** - คุณต้องตรวจสอบให้แน่ใจว่าอุปกรณ์มีโทเค็นรีเฟรชหลักของ Azure AD (PRT) For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

เมื่อต้องการตรวจสอบว่าคุณมี Azure AD PRT หรือไม่ คุณสามารถเรียกใช้สั่งบนอุปกรณ์ และตรวจสอบว่า `dsregcmd/status` "AzureAdPrt" เท่ากับ "YES" หรือไม่

ถ้า "AzureAdPrt" เป็น "NO" ให้ตรวจสอบดังต่อไปนี้:

- **ไม่ว่าคุณจะ** มีสภาพแวดล้อมภายนอกกับ AD FS และไม่สามารถเข้าถึงได้จากเครือข่ายหลักของผู้ใช้ของคุณ : ในกรณีนี้ ตรวจสอบให้แน่ใจว่าจุดสิ้นสุด "usernamemixed" ของคุณสามารถเข้าถึงได้จากเอกซ์ทราเน็ต ถ้า AD FS ของคุณอยู่หลัง VPN ตรวจสอบให้แน่ใจว่าผู้ใช้เชื่อมต่อกับ VPN และลงชื่อเข้าใช้อุปกรณ์อีกครั้ง ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)นี้

- **TPM ของอุปกรณ์** เป็นข้อผิดพลาดหรือไม่ และไม่สามารถรับรองความถูกต้องของอุปกรณ์ได้ : ตรวจสอบ "tpm.msc" เพื่อดูว่าสถานะของ TPM เป็น "พร้อมแล้ว" หรือไม่ ถ้าไม่ ให้ `dsregcmd/leave` เรียกใช้และให้อุปกรณ์เข้าร่วมกับ Azure AD อีกครั้ง จากนั้นลองอีกครั้ง ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)นี้

- **คุณใช้งานผู้ให้บริการข้อมูลเฉพาะตัวของบริษัทอื่น ซึ่งไม่สนับสนุนWS-Trustโพรโทคอล** ตามที่อธิบายไว้ในเอกสารของเรา อุปกรณ์ที่เข้าร่วม Azure AD แบบไฮบริดจะไม่สามารถใช้งานในกรณีนี้ได้ โปรดติดต่อผู้ให้บริการข้อมูลเฉพาะตัวของคุณเพื่อรับการสนับสนุน

2. ผู้ใช้ใช้เบราว์เซอร์ Chrome โดยไม่มีบัญชี **Windows 10** หรือ Chrome ส่วนขยาย Office จะไม่ใช้ PRT บนอุปกรณ์ที่เข้าร่วม **ด้วย AAD** หรืออุปกรณ์ที่เข้าร่วมแบบไฮบริดโดยอัตโนมัติ: ซึ่งไปสู่ความล้มเหลวในการนโยบายการเข้าถึงตามเงื่อนไขบนอุปกรณ์ใดๆ ที่มีข้อความแสดงข้อผิดพลาด "อุปกรณ์ที่ไม่ได้ลงทะเบียน" แสดงขึ้น เมื่อต้องการใช้เบราว์เซอร์ Chrome อย่างถูกต้อง คุณต้องติดตั้ง "บัญชี Windows 10" หรือ "ส่วนขยาย Office ไปยังเบราว์เซอร์ Chrome ของผู้ใช้" ผ่าน SCCM หรือ Intun e ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)นี้

ถ้าไม่สามารถส่งส่วนขยายระยะไกลได้ ให้แจ้งให้ผู้ใช้ติดตั้งส่วนขยายข้างต้นด้วยตนเองเพื่อเข้าถึงแอปพลิเคชันที่อยู่เบื้องหลังการเข้าถึงตามเงื่อนไขบนอุปกรณ์ ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)นี้

3. อุปกรณ์ถูกรวม Azure AD แบบไฮบริดอย่างถูกต้อง แต่ถูกลบหรือปิดใช้งานโดยไม่ได้ตั้งใจ ไม่ว่าจะเกิดจากการซิงค์การเปลี่ยนแปลงใน **Azure AD Connect** หรือจากพอร์ทัล Azure : ในกรณีนี้ วัตถุอุปกรณ์จะไม่ถูกรับรู้ว่าเป็นอุปกรณ์ที่เข้าร่วมโดยสมบูรณ์อีกต่อไป แม้ว่าสถานะ "AzureAdJoined" และ "PRT" จะแสดงอย่างถูกต้องบนอุปกรณ์

เมื่อต้องการแก้ไขปัญหานี้ ให้เรียกใช้ `dsregcmd/leave` บนอุปกรณ์ที่ได้รับผลกระทบและให้พวกเขาเข้าร่วม Azure AD อีกครั้ง ดูข้อมูลเพิ่มเติมที่ [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)นี้

> [!NOTE]
> ถ้าอุปกรณ์ของคุณอยู่ในการอัปเดต Windows 10, 1809 ด้วยพร็อกซี VPN/Cloud และดูปัญหาเกี่ยวกับ "AzureAdPrt" หรือแอปใดๆ ที่มีปัญหา SSO (Outlook ไม่ได้เชื่อมต่อกับกล่องจดหมายแม้ว่าคุณจะมี PRT) ตรวจสอบให้แน่ใจว่าคุณมีโปรแกรมแก้ไข [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) หรือการอัปเดตสะสมในเดือนเมษายน [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) เพื่อป้องกันการ PRT ล้มเหลวบนเครื่องเหล่านั้น

















