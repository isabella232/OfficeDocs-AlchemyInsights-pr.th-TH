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
ms.openlocfilehash: d71bb376615191f507d39b99d9e51ca77d929b90
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323457"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>ฉันถูกบล็อกโดยการเข้าถึงตามเงื่อนไขด้วยอุปกรณ์ที่เข้าร่วมในโดเมน

**เครื่องมือที่แนะนาเป็นอย่างยิ่ง**

[เครื่องมือแก้ไขปัญหาการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - เครื่องมือที่ช่วยในการแก้ไขปัญหาการลงทะเบียนอุปกรณ์ที่พบบ่อยที่สุด

[ทดสอบสคริปต์การเชื่อมต่อการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - สคริปต์ที่ช่วยรับรองว่าอุปกรณ์สามารถเข้าถึงจุดสิ้นสุดการลงทะเบียนอุปกรณ์ภายใต้บัญชีระบบ

[สคริปต์การล้างข้อมูลอุปกรณ์ Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - สคริปต์ที่ช่วยให้คุณสามารถค้นหาและจัดการอุปกรณ์เก่าในสภาพแวดล้อมของคุณ

ต่อไปนี้เป็นสาเหตุทั่วไปบางประการที่การเข้าถึงตามเงื่อนไขอาจล้มเหลวอุปกรณ์ที่เข้าร่วมโดเมน (Azure AD แบบไฮบริด)

1. **ไม่มี Azure AD PRT บนอุปกรณ์** - คุณต้องตรวจสอบให้แน่ใจว่าอุปกรณ์มีโทเค็นรีเฟรชหลัก Azure AD (PRT) For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

เมื่อต้องการตรวจสอบว่าคุณมี PrT ของ Azure AD หรือไม่ คุณสามารถเรียกใช้สั่งบนอุปกรณ์และ `dsregcmd/status` ตรวจสอบว่า "AzureAdPrt" เท่ากับ "YES" หรือไม่

ถ้า "AzureAdPrt" เป็น "NO" ให้ตรวจสอบดังต่อไปนี้:

- **ไม่ว่าคุณจะมีสภาพแวดล้อม** ภายนอกกับ AD FS และไม่สามารถเข้าถึงจากเครือข่ายหลักของผู้ใช้ของคุณ : ในกรณีนี้ ตรวจสอบให้แน่ใจว่า จุดสิ้นสุด "usernamemixed" ของคุณสามารถเข้าถึงได้จากเอกซ์ทราเน็ต ถ้า AD FS ของคุณอยู่ด้านหลัง VPN ตรวจสอบให้แน่ใจว่าผู้ใช้เชื่อมต่อกับ VPN และเข้าสู่ระบบอีกครั้งกับอุปกรณ์ หากต้องการข้อมูลเพิ่มเติม โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)นี้

- **TPM ของอุปกรณ์เป็นข้อผิดพลาด** หรือไม่ และไม่สามารถรับรองความถูกต้องของอุปกรณ์ : ตรวจสอบ "tpm.msc" เพื่อดูว่าสถานะของ TPM เป็น "พร้อมแล้ว" หรือไม่ หากไม่ ให้ `dsregcmd/leave` เรียกใช้และให้อุปกรณ์เข้าร่วมกับ Azure AD อีกครั้ง จากนั้นลองอีกครั้ง หากต้องการข้อมูลเพิ่มเติม โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)นี้

- **คุณใช้งานผู้ให้บริการข้อมูลเฉพาะตัวของบริษัทอื่น ซึ่งไม่สนับสนุนWS-Trustโพรโทคอล** ตามที่อธิบายไว้ในเอกสารของเรา อุปกรณ์ที่เข้าร่วมด้วย Azure AD แบบไฮบริดจะไม่สามารถใช้งานในกรณีนี้ได้ โปรดติดต่อผู้ให้บริการข้อมูลเฉพาะตัวของคุณเพื่อรับการสนับสนุน

2. ผู้ใช้ใช้เบราว์เซอร์ Chrome ที่ไม่มี **บัญชี Windows 10** หรือ Chrome ส่วนขยาย Office จะไม่ใช้ PRT บนอุปกรณ์ที่เข้าร่วม AAD หรืออุปกรณ์ที่เข้าร่วม **AAD** แบบไฮบริดโดยอัตโนมัติ: ซึ่งไปสู่ความล้มเหลวของนโยบายการเข้าถึงตามเงื่อนไขบนอุปกรณ์ใดๆ ที่มีข้อความแสดงข้อผิดพลาด "อุปกรณ์ที่ไม่ได้ลงทะเบียน" แสดงขึ้น เมื่อต้องการใช้เบราว์เซอร์ Chrome อย่างถูกต้อง คุณต้องติดตั้ง "บัญชี Windows 10" หรือ "Office ส่วนขยาย Office เบราว์เซอร์ Chrome ของผู้ใช้" ผ่าน SCCM หรือ Intun e หากต้องการข้อมูลเพิ่มเติม โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)นี้

ถ้าไม่สามารถส่งส่วนขยายจากระยะไกลได้ แจ้งให้ผู้ใช้ติดตั้งส่วนขยายข้างต้นด้วยตนเองเพื่อเข้าถึงแอปพลิเคชันที่อยู่เบื้องหลังการเข้าถึงตามเงื่อนไขบนอุปกรณ์ หากต้องการข้อมูลเพิ่มเติม โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)นี้

3. อุปกรณ์ถูกรวม Azure AD แบบไฮบริดอย่างถูกต้อง แต่ถูกลบหรือปิดใช้งานโดยไม่ได้ตั้งใจ ไม่ว่าจะเนื่องจากการซิงค์การเปลี่ยนแปลงใน **Azure AD เชื่อมต่อ** หรือจากพอร์ทัล Azure : ถ้าเกิดกรณีนี้ขึ้น วัตถุอุปกรณ์จะไม่รับรู้เป็นอุปกรณ์ที่เข้าร่วมอย่างสมบูรณ์อีกต่อไป แม้ว่าสถานะ "AzureAdJoined" และ "PRT" จะแสดงเป็นใช้งานได้บนอุปกรณ์

เมื่อต้องการแก้ไขปัญหานี้ ให้เรียกใช้ `dsregcmd/leave` บนอุปกรณ์ที่ได้รับผลกระทบและให้พวกเขาเข้าร่วม Azure AD อีกครั้ง หากต้องการข้อมูลเพิ่มเติม โปรดดู [เอกสาร](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)นี้

**หมายเหตุ**: ถ้าอุปกรณ์ของคุณอยู่ใน Windows 10 การอัปเดต 1809 ด้วยพร็อกซี VPN/Cloud และดูปัญหาเกี่ยวกับสถานะ "AzureAdPrt" หรือแอปใดๆ ที่มีปัญหา SSO (Outlook ไม่ได้เชื่อมต่อกับกล่องจดหมายแม้ว่าคุณจะมี PRT) ตรวจสอบให้แน่ใจว่าคุณมีโปรแกรมแก้ไข [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2)หรือการอัปเดตสะสมในเดือนเมษายน [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6)เพื่อป้องกันการ PRT ที่ล้มเหลวบนเครื่องเหล่านั้น

















