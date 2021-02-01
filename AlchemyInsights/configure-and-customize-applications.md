---
title: กําหนดค่าและกําหนดค่าแอปพลิเคชัน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063711"
---
# <a name="configure-and-customize-applications"></a>กําหนดค่าและกําหนดค่าแอปพลิเคชัน

**กําหนดค่าแอปพลิเคชัน**

1. [การเริ่มต้นใช้งานด่วน: การกําหนดค่าคุณสมบัติแอปพลิเคชันในผู้เช่า Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) จะแสดงวิธีการกําหนดค่าคุณสมบัติบางอย่างของแอป
2. เพื่อช่วยรวมแอปพลิเคชันของคุณเข้ากับ Azure Active Directory เราได้พัฒนาคอลเลกชันของบท [ช่วย](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) สอนที่จะช่วยคุณผ่านการกําหนดค่า
3. [วิธีการกําหนดค่าแอปพลิเคชันพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) ช่วยให้คุณเข้าใจวิธีการกําหนดค่าแอปพลิเคชันพร็อกซีแอปพลิเคชันภายใน Azure AD เพื่อแสดงแอปพลิเคชันภายในองค์กรของคุณไปยัง Cloud
4. [ดาวน์โหลด PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)และกําหนดค่าแอปพลิเคชันของคุณ: ให้ปฏิบัติตามคําแนะนําใน กําหนดค่า *PingAccess* for Azure AD เพื่อป้องกันแอปพลิเคชันที่เผยแพร่โดยใช้พร็อกซีแอปพลิเคชัน Microsoft Azure AD บนเว็บไซต์ข้อมูลเฉพาะตัวของ Ping และดาวน์โหลด PingAccess เวอร์ชันล่าสุด

**ข้อผิดพลาดของแอปพลิเคชันที่ตั้งค่าผิด (AADSTS650056)**

1. ตรวจสอบให้แน่ใจว่าคุณเข้าถึงแอปพลิเคชันจากที่อยู่การลงชื่อเข้าใช้ที่ให้มาโดยเจ้าของแอปพลิเคชัน มิฉะนั้นความหมาย ให้ลงชื่อเข้าใช้แอปพลิเคชันผ่านกระบวนการปกติ ในกรณีส่วนใหญ่ สิ่งนี้จะแก้ไขโดยอัตโนมัติอย่างเป็นธรรมชาติ ถ้าไม่ โพสต์นี้สามารถช่วยแก้ไขปัญหาได้
2. **ถ้าองค์กรของคุณเป็นเจ้าของแอปพลิเคชัน** (หมายความว่าการลงทะเบียนแอปพลิเคชันอยู่ในองค์กรของคุณ):
    - อย่างน้อยที่สุด เราแนะน `User.Read` า `openid` ให้เพิ่มสิทธิ์หรือที่ได้รับมอบสิทธิ์จาก **Microsoft Graph** แล้ว
    - ตรวจสอบให้แน่ใจว่าแอปพลิเคชันและสิทธิ์ทั้งหมดได้รับความยินยอม คุณสามารถตรวจสอบได้โดยดูที่ **คอลัมน์สถานะของการลงทะเบียน** แอปพลิเคชันภายใน **สิทธิ์ API**
    - ในบางสถานการณ์ แอปพลิเคชันอาจของบริษัทอื่น แต่อาจลงทะเบียนในองค์กรของคุณ ยืนยันถ้าแอปพลิเคชันนี้แสดงอยู่ในการลงทะเบียนแอปของคุณ (ไม่ใช่แอปพลิเคชันระดับองค์กร)
    - ถ้าคุณยังคงเห็นข้อความแสดงข้อผิดพลาดนี้ จากนั้น คุณอาจต้องสร้าง URL ความยินยอมที่อธิบายไว้ใน **ขั้นตอนที่ 4**
3. **ถ้าองค์กรของคุณไม่ได้เป็นเจ้าของแอปพลิเคชันและใช้เป็นแอปพลิเคชันของบริษัทอื่น** ให้:
    - ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง/บริษัท คุณควรเห็นหน้าจอความยินยอม ตรวจสอบให้แน่ใจว่าคุณได้เลือกกล่อง **"ความยินยอมในนามขององค์กรของคุณ"**
    - ถ้าคุณไม่เห็นหน้าจอความยินยอม ให้ลบแอปพลิเคชัน Enterprise แล้วลองอีกครั้ง
    - ถ้าคุณยังคงเห็นข้อความแสดงข้อผิดพลาดนี้ จากนั้น คุณอาจต้องสร้าง URL ความยินยอมที่อธิบายไว้ใน **ขั้นตอนที่ 4**
4. **สร้าง URL** การยินยอมด้วยตนเองที่จะใช้ : ถ้าแอปพลิเคชันออกแบบมาเพื่อเข้าถึงทรัพยากรเฉพาะ คุณอาจไม่สามารถใช้ปุ่มการยินยอมจากพอร์ทัล Azure คุณจะต้องสร้าง URL การยินยอมของคุณเองและใช้ URL นี้ด้วยตนเอง
    - คุณจะต้องได้รับ `{App-Id}` และ `{App-Uri-Id}` จากเจ้าของแอปพลิเคชัน `{Tenant-Id}` จะเป็นตัวระบุผู้เช่าของคุณ ซึ่งจะเป็นหรือ `yourdomain.onmicrosoft.com` ID ไดเรกทอรีของคุณ
    - If the application is accessing itself for the resource, then `{App-Id}` the and will be `{App-Uri-Id}` same.
5. For more information, see [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**การปรับแต่งแอปพลิเคชัน**

- [เพิ่มตรา](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) สินค้าลงในหน้าลงชื่อเข้าใช้ Azure Active Directory ขององค์กรของคุณ - ใช้โลโก้ขององค์กรของคุณและแบบแผนชุดสีแบบปรับแต่งเองเพื่อให้หน้าลงชื่อเข้าใช้ Azure Active Directory (Azure AD) มีลักษณะสอดคล้องกัน
- [เพิ่มชื่อโดเมนแบบปรับแต่งเองของคุณโดยใช้พอร์ทัล Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - ผู้เช่า Azure AD ใหม่ทุกรายจะมาพร้อมกับชื่อโดเมนเริ่มต้น คุณไม่สามารถเปลี่ยนหรือลบชื่อโดเมนเริ่มต้น แต่คุณสามารถเพิ่มชื่อองค์กรของคุณได้ การเพิ่มชื่อโดเมนแบบปรับแต่งเองจะช่วยให้คุณสร้างชื่อผู้ใช้ที่คุ้นเคยกับผู้ใช้ของคุณ
