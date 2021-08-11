---
title: การแก้ไขปัญหาผู้ใช้
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: 0c4ee54a6f1d00e7fd3794539ba185afa4327af1124d8057550806f7fa87de7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54092969"
---
# <a name="announcements"></a>ประกาศ

ปฏิบัติตามแนวทางของ Google เกี่ยวกับการทดสอบความเข้ากันได้เพื่อทดสอบว่าแอปของคุณได้รับผลกระทบหรือไม่ มีแนวทางของ Google https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support อยู่ใน

ตรวจสอบให้แน่ใจว่าคุณใช้มุมมองเว็บของระบบหรือเบราว์เซอร์ระบบเมื่อลงชื่อเข้าใช้ผู้ใช้ของคุณด้วยบัญชี Google ของลูกค้า For more information, [see Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**ฉันไม่สามารถสร้างผู้ใช้ใหม่ในไดเรกทอรี Azure AD ของฉัน**

เมื่อต้องการแก้ไขปัญหาไม่สามารถสร้างผู้ใช้ใหม่ใน Azure AD ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างผู้ใช้มาตรฐานใหม่ เฉพาะบทบาทผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบผู้ใช้ใน Azure Active Directory (AD) เท่านั้นที่สามารถสร้างผู้ใช้มาตรฐานใหม่ได้ ถ้าคุณไม่ได้อยู่ในบทบาทใดบทบาทหนึ่ง ให้ขอให้ผู้ดูแลระบบเพิ่มคุณลงในบทบาทเหล่านี้ หรือสร้างบัญชีผู้ใช้ใหม่ให้คุณ
2. ตรวจสอบให้แน่ใจว่าชื่อผู้ใช้อยู่ในโดเมนที่ได้รับการยืนยันใน Azure AD ของคุณ ถ้าคุณไม่มีชื่อโดเมนแบบปรับแต่งเองที่ตรวจสอบแล้วใน Azure AD คุณสามารถใช้โดเมนเริ่มต้น Azure AD ของคุณ ซึ่งลงท้ายด้วย *.onmicrosoft.com
3. ตรวจสอบให้แน่ใจว่าชื่อผู้ใช้อยู่ในโดเมนที่ไม่ได้ติดต่อกับภายนอก Azure AD จาก AD ภายในองค์กรของคุณ ผู้ใช้ไม่สามารถเพิ่มในระบบคลาวด์ด้วยชื่อโดเมนที่ติดต่อกับภายนอกจากภายในองค์กรได้
4. ตรวจสอบให้แน่ใจว่าไม่มีผู้ใช้หรือที่ติดต่ออื่นมีชื่อผู้ใช้ที่คุณต้องการกําหนดให้กับผู้ใช้ใหม่แล้ว ชื่อผู้ใช้ต้องไม่ซ.ก. ใน Azure AD
5. ดู [บทบาทและผู้ดูแลระบบ Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ของ Azure AD
6. ดู [ชื่อโดเมนของ](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) Azure AD ของคุณ
7. ตรวจทาน [บันทึก](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) การตรวจสอบเพื่อดูข้อมูลโดยละเอียดเพิ่มเติมเกี่ยวกับผู้ใช้ที่สร้างหรือผู้ใช้ที่ถูกลบเมื่อเร็วๆ นี้ เช่น ผู้ที่เป็นผู้ปฏิบัติการและเมื่อใด
8. For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. For more information on administrator role permissions in Azure AD, see [Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. For details on creating a user using Azure AD Powershell, see [Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**ปัญหาในการลงทะเบียนด้วยตนเอง**

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการลงทะเบียนด้วยตนเอง ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. เมื่อต้องการใช้การลงทะเบียนด้วยตนเองกับแอปพลิเคชันของคุณ ก่อนอื่นให้เปิดใช้งานการลงทะเบียนด้วยตนเองให้กับผู้เช่าของคุณ 
2. เมื่อต้องการเปิดใช้งานแอปพลิเคชันเพื่อสนับสนุนการลงทะเบียนด้วยตนเอง ให้เพิ่มลงในโฟลว์ผู้ใช้ของคุณ ในครั้งถัดไปที่คุณไปที่หน้าลงชื่อเข้าใช้ของแอปพลิเคชันนั้น คุณจะเห็นตัวเลือก ***ไม่มีบัญชี ใช่ไหม สร้างบัญชีเลย*** ซึ่งจะเริ่มกระบวนการลงทะเบียนด้วยตนเอง
3. For information on how to use self-service sign up to populated an organization in Azure AD, see [Self-service sign up for Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. เมื่อคุณเชื่อมโยงโฟลว์ผู้ใช้กับแอปพลิเคชันอย่างน้อยหนึ่งรายการ ผู้ใช้ที่เยี่ยมชมแอปนั้นจะสามารถลงทะเบียนและได้รับบัญชี Guest โดยใช้ตัวเลือกที่กําหนดค่าในขั้นตอนของผู้ใช้ For more information on sign up and gaining a guest account, the users can see [Self-service sign-up for guest users](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

**ปัญหาในการเชิญผู้ใช้ภายนอก**

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการเชิญผู้ใช้ภายนอก ให้ปฏิบัติตามขั้นตอนต่อไปนี้

ตรวจสอบให้แน่ใจว่าคุณได้ส่งคําเชิญของผู้ใช้ไปยังที่อยู่อีเมลที่ตรงกับชื่อที่ผู้ใช้ลงชื่อเข้าใช้ If you send the invitation to a user's proxy email address, the user can't redeem it. หากต้องการข้อมูลเพิ่มเติม โปรดดูคู่มือ[Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/)

**ฉันไม่สามารถกําหนดสิทธิ์การใช้งานให้กับผู้ใช้ได้**

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับการกําหนดสิทธิ์การใช้งานให้กับผู้ใช้ ให้ปฏิบัติตามขั้นตอนต่อไปนี้

1. เมื่อต้องการจัดการสิทธิ์การใช้งานของผู้ใช้ ตรวจสอบให้แน่ใจว่าคุณใช้บัญชีผู้ใช้กับบทบาทผู้ดูแลระบบที่ต้องมีบทบาทใดบทบาทหนึ่ง ได้แก่ ผู้ดูแลระบบส่วนกลาง ผู้ดูแลสิทธิ์การใช้งาน หรือผู้ดูแลระบบผู้ใช้ คุณสามารถตรวจสอบบทบาทของผู้ใช้ในแท็บ **บทบาท** ไดเรกทอรี บน Blade ผู้ใช้ได้
2. ถ้าคุณใช้งานพอร์ทัล Azure และการมอบหมายสิทธิ์การใช้งานล้มเหลว ให้คลิกการแจ้งเตือนที่มุมขวาบน ซึ่งจะเปิดใบที่มีรายละเอียดเกี่ยวกับสิ่งที่ผิดพลาด ในกรณีส่วนใหญ่ที่เข้าใจและแก้ไขปัญหาได้
3. ก่อนที่จะมอบหมายสิทธิ์การใช้งานให้กับผู้ใช้ ตรวจสอบให้แน่ใจว่าคุณ **ตั้งค่าคุณสมบัติ** สถานที่การใช้งาน ไว้ให้กับผู้ใช้แล้ว ตรวจสอบว่าผู้ใช้มีการตั้งค่าคุณสมบัตินั้นโดยการ **ดู** แท็บ โปรไฟล์ บนเบลดของผู้ใช้
4. ตรวจสอบให้แน่ใจว่ามีสิทธิ์การใช้งานที่พร้อมใช้งานเพียงพอของผลิตภัณฑ์ที่คุณพยายามกําหนด คุณสามารถดูจํานวนสิทธิ์การใช้งานที่พร้อมใช้งานในพอร์ทัล Azure ได้ที่ Azure Active Directory [->สิทธิ์การใช้งาน -> ผลิตภัณฑ์](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)ทั้งหมด
5. ผู้ใช้อาจมีสิทธิ์การใช้งานอื่นที่บริการขัดแย้งกับสิทธิ์ในสิทธิ์การใช้งานใหม่ที่คุณพยายามกําหนด For example, if the user has the Exchange Online (Plan 1) service enabled, you won't able to assign a license with the Exchange Online (Plan 2). ปิดใช้งานหนึ่งในบริการเพื่ออนุญาตการมอบหมายสิทธิ์การใช้งานใหม่ ถ้าคุณใช้พอร์ทัล Azure หรือ cmdlet ของ PowerShell **หน้ารายละเอียด** ปัญหาจะแสดงรายการบริการเฉพาะที่ทําให้เกิดข้อขัดแย้ง
6. If you are trying to remove a license and that is failing, the user might have other licenses with services that depend on the services you are trying to remove. ถ้าคุณใช้พอร์ทัล Azure หรือ cmdlet ของ PowerShell ข้อความแสดงข้อผิดพลาดจะแสดงรายการบริการเฉพาะที่ขึ้นต่อกัน
7. ถ้าคุณต้องการเข้าใจว่าเหตุใดสิทธิ์การใช้งานจึงถูกเพิ่ม/เอาออกจากผู้ใช้ (ตัวอย่างเช่น บุคคลอื่นในองค์กรของคุณอาจมีการเปลี่ยนแปลงบ้าง) ให้ตรวจสอบบันทึกการตรวจสอบ ตั้งค่าตัวกรองเป็น **กิจกรรมสิทธิ์การใช้งาน** เพื่อแสดงการปรับเปลี่ยนทั้งหมด รวมถึง "actor" ที่ปฏิบัติการปรับเปลี่ยนเหล่านั้น
8. ถ้าคุณใช้งาน Exchange Online ผู้ใช้บางรายในผู้เช่าของคุณอาจถูกกําหนดค่าอย่างไม่ถูกต้องด้วยค่าที่อยู่พร็อกซีเดียวกัน ในกรณีดังกล่าว คุณอาจเห็นข้อความแสดงข้อผิดพลาดทั่วไปเมื่อการดําเนินการสิทธิ์การใช้งานล้มเหลว [บทความนี้](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used)ประกอบด้วยข้อมูลเพิ่มเติมเกี่ยวกับปัญหานี้ รวมถึงข้อมูลเกี่ยวกับ[วิธีการเชื่อมต่อกับExchange Onlineโดยใช้ PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)ระยะไกล เมื่อต้องการระบุผู้ใช้ในผู้เช่าของคุณ ให้ใส่ที่อยู่พร็อกซีเดียวกัน ให้เรียกใช้ cmdlet Exchange Onlineต่อไปนี้

เรียกใช้

Get-Recipient | เมื่อ {$_ EmailAddresses -match <user principal name> } | fL Name, RecipientType,emailaddresses





