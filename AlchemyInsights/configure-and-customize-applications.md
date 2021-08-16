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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045007"
---
# <a name="configure-and-customize-applications"></a>กําหนดค่าและกําหนดค่าแอปพลิเคชัน

**กําหนดค่าแอปพลิเคชัน**

1. [การเริ่มต้นใช้งานด่วน: กําหนดค่าคุณสมบัติแอปพลิเคชันในผู้เช่า Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)ของคุณแสดงวิธีการกําหนดค่าคุณสมบัติบางอย่างของแอป
2. เพื่อช่วยรวมแอปพลิเคชันของคุณเข้ากับAzure Active Directoryต่างๆ เราได้พัฒนาคอลเลกชันของ[บทช่วย](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)สอนที่จะช่วยคุณตลอดการกําหนดค่า
3. [วิธีการกําหนดค่าแอปพลิเคชันพร็อกซีแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) ช่วยให้คุณเข้าใจวิธีกําหนดค่าแอปพลิเคชันพร็อกซีแอปพลิเคชันภายใน Azure AD เพื่อแสดงแอปพลิเคชันภายในองค์กรของคุณไปยังระบบคลาวด์
4. [ดาวน์โหลด PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)และกําหนดค่าแอปพลิเคชันของคุณ: ให้ปฏิบัติตามคําแนะนําใน กําหนดค่า *PingAccess* for Azure AD เพื่อป้องกันแอปพลิเคชันที่ประกาศโดยใช้ Microsoft Azure AD Application Proxy บนเว็บไซต์ข้อมูลเฉพาะตัวของ Ping และดาวน์โหลด PingAccess เวอร์ชันล่าสุด

**ข้อผิดพลาดแอปพลิเคชันที่ปรับแต่งผิด (AADSTS650056)**

1. ตรวจสอบให้แน่ใจว่าคุณเข้าถึงแอปพลิเคชันจากที่อยู่การลงชื่อเข้าใช้ที่เจ้าของแอปพลิเคชันจัดหาให้ มิฉะนั้นให้ลงชื่อเข้าใช้แอปพลิเคชันผ่านกระบวนการปกติ ในกรณีส่วนใหญ่ การแก้ไขอัตโนมัติจะเป็นธรรมชาติ ถ้าไม่ โพสต์นี้สามารถช่วยแก้ไขปัญหาได้
2. **ถ้าองค์กรของคุณเป็นเจ้าของแอปพลิเคชัน** (หมายความว่าการลงทะเบียนแอปพลิเคชันอยู่ในองค์กรของคุณ):
    - อย่างน้อยที่สุด เราขอแนะ `User.Read` Graph `openid` หรือมอบสิทธิ์จาก **Microsoft**
    - ตรวจสอบให้แน่ใจว่าแอปพลิเคชันและสิทธิ์ทั้งหมดได้รับความยินยอม คุณสามารถตรวจสอบได้โดยดูที่คอลัมน์ **สถานะ ของ** การลงทะเบียนแอปพลิเคชันภายใน **สิทธิ์ API**
    - ในบางสถานการณ์ แอปพลิเคชันอาจไม่ใช่บริษัทอื่น แต่อาจได้รับการลงทะเบียนในองค์กรของคุณ ยืนยันถ้าแอปพลิเคชันนี้แสดงอยู่ในการลงทะเบียนแอปของคุณ (แอปพลิเคชัน Not Enterprise)
    - ถ้าคุณยังคงเห็นข้อความแสดงข้อผิดพลาดนี้ จากนั้น คุณอาจต้องสร้าง URL การยินยอมที่อธิบายไว้ใน **ขั้นตอนที่ 4**
3. **หากองค์กรของคุณไม่ใช่เจ้าของแอปพลิเคชันและใช้แอปพลิเคชันเป็นแอปพลิเคชันของบริษัทอื่น**:
    - หากคุณเป็นผู้ดูแลระบบส่วนกลาง/บริษัท คุณควรเห็นหน้าจอความยินยอม ตรวจสอบให้แน่ใจว่าคุณได้เลือกกล่อง **"ความยินยอมในนามขององค์กรของคุณ"**
    - ถ้าคุณไม่เห็นหน้าจอความยินยอม ให้ลบแอปพลิเคชัน Enterprise แล้วลองอีกครั้ง
    - ถ้าคุณยังคงเห็นข้อความแสดงข้อผิดพลาดนี้ จากนั้น คุณอาจต้องสร้าง URL การยินยอมที่อธิบายไว้ใน **ขั้นตอนที่ 4**
4. **สร้าง URL** การยินยอมด้วยตนเองเพื่อใช้ : ถ้าแอปพลิเคชันออกแบบมาเพื่อเข้าถึงทรัพยากรเฉพาะ คุณอาจไม่สามารถใช้ปุ่ม การยินยอม จากพอร์ทัล Azure คุณจะต้องสร้าง URL การยินยอมของคุณเอง และใช้สิ่งนี้
    - คุณจะต้องได้รับ `{App-Id}` และ จาก `{App-Uri-Id}` เจ้าของแอปพลิเคชัน `{Tenant-Id}` จะเป็นตัวระบุผู้เช่าของคุณ ซึ่งจะเป็นหรือ `yourdomain.onmicrosoft.com` ID ไดเรกทอรีของคุณ
    - ถ้าแอปพลิเคชันเข้าถึงทรัพยากรเอง แล้ว `{App-Id}` `{App-Uri-Id}` และ จะเป็นแบบเดียวกัน
5. For more information, see [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**การปรับแต่งแอปพลิเคชัน**

- [เพิ่มตรา](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding)สินค้าในหน้าลงชื่อเข้าใช้ Azure Active Directory ขององค์กรของคุณ - ใช้โลโก้ขององค์กรของคุณและแบบแผนชุดสีแบบปรับแต่งเองเพื่อให้หน้าลงชื่อเข้าใช้ Azure Active Directory (Azure AD) ของคุณสอดคล้องกัน
- [เพิ่มชื่อโดเมนแบบปรับแต่งเองของคุณโดยใช้Azure Active Directoryโดเมนของคุณ](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain)- ผู้เช่า Azure AD ใหม่ทุกรายจะมาพร้อมกับชื่อโดเมนเริ่มต้น คุณไม่สามารถเปลี่ยนหรือลบชื่อโดเมนเริ่มต้น แต่คุณสามารถเพิ่มชื่อองค์กรของคุณได้ การเพิ่มชื่อโดเมนแบบปรับแต่งเองจะช่วยให้คุณสามารถสร้างชื่อผู้ใช้ที่คุ้นเคยจากผู้ใช้ของคุณ
