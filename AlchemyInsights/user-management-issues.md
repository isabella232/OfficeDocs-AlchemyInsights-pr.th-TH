---
title: ปัญหาการจัดการผู้ใช้
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
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037511"
---
# <a name="user-management-issues"></a>ปัญหาการจัดการผู้ใช้

**What happens to current assigned users to the application if I disable the property 'User assignment required' (set this property to No)?**

การปิดใช้งาน **การมอบหมายของผู้ใช้** ที่ต้องใช้จะไม่มีผลต่อผู้ใช้ที่ได้รับมอบหมายในปัจจุบัน การปิดใช้งานคุณสมบัตินี้จะอนุญาตให้ผู้ใช้ทั้งหมดเข้าถึงแอปพลิเคชันได้เท่านั้น ผู้ใช้ที่แสดงอยู่ในรายการและผู้ใช้ที่ได้รับการมอบหมายให้กลุ่มในแอปพลิเคชันจะยังคงใช้งานได้

- เมื่อต้องการจํากัดแอปของคุณเฉพาะกลุ่มผู้ใช้ ให้ดู -[จํากัดแอป Azure AD เป็นชุดของผู้ใช้ - แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)
- เมื่อต้องการกําหนดผู้ใช้และกลุ่ม ให้กับแอปพลิเคชันขององค์กรใน Azure Active Directory (Azure AD) จากภายในพอร์ทัล Azure หรือโดยใช้ PowerShell ให้ดู จัดการงานที่มอบหมายของผู้ใช้ในแอป[ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- เมื่อต้องการมอบสิทธิ์การสร้างและการจัดการแอปพลิเคชัน ให้ดู[มอบสิทธิ์ผู้ดูแลระบบแอปพลิเคชันในฐานะผู้รับมอบสิทธิ์ - Azure AD | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)
- **ซ่อนแอปองค์กรที่เฉพาะเจาะจงจากผู้ใช้**- ใช้ขั้นตอนต่อไปนี้เพื่อซ่อนแอป Microsoft 365 ทั้งหมดจาก **แผง MyApps** แอปจะยังคงมองเห็นได้ในพอร์ทัล Office 365

 1. ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบส่วนกลางของไดเรกทอรีของคุณ 
 2. เลือก **Azure Active Directory** 
 3. เลือก **ผู้ใช้** 
 4. เลือก **การตั้งค่า** ผู้ใช้ 
 5. ภายใต้ **แอปพลิเคชัน** ขององค์กร ให้คลิก **จัดการวิธีเปิดใช้และดูแอปพลิเคชันของผู้ใช้** 
 6. For **Users can only see Office 365 apps in the Office 365 portal,** click **Yes**. 
 7. คลิก **บันทึก** 
 8. For more details, see [Hide an Enterprise application from user's experience in Azure AD | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- ถ้าคุณเสนอแอปซอฟต์แวร์เป็นบริการ (SaaS) ให้กับองค์กรมากมาย คุณสามารถกําหนดค่าแอปให้ยอมรับการลงชื่อเข้าใช้จากผู้เช่า Azure Active Directory (Azure AD) ใดก็ได้ การกําหนดค่านี้เรียกว่า "การกําหนดให้แอปพลิเคชันของคุณมีหลายผู้เช่า" ผู้ใช้ในผู้เช่า Azure AD จะสามารถลงชื่อเข้าใช้แอปของคุณหลังจากยินยอมให้ใช้บัญชีของพวกเขากับแอปของคุณ For more information, see [build apps that sign in Azure AD users - Microsoft identity platform | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)

- **ผู้ใช้ปลายทางจะสามารถเข้าถึงแอปพลิเคชันได้อย่างไรเมื่อเขา/เธอถูกมอบหมายไปยังแอปพลิเคชัน**

แต่ละแอปในใบแอปพลิเคชัน Enterprise จะมีลิงก์เพื่อให้ผู้ใช้เข้าถึงได้ ผู้ใช้ยังสามารถเข้าถึงแอปผ่าน **พอร์ทัลแอป** ของฉันด้วยวิธีง่ายๆ

- **ต้องการทราบว่าผู้ใช้ใช้งานแอปพลิเคชันและแอปพลิเคชันชนิดใดอยู่หรือไม่**

คุณสามารถดาวน์โหลดรายงานการลงชื่อเข้าใช้ในช่วง 30 วันที่ผ่านมาได้จาก **portal.azure.com > Azure Active Directory>ลงชื่อเข้าใช้>ดาวน์โหลดรายงาน**

- เรียนรู้วิธีการให้ความยินยอม[จากผู้ดูแลระบบทั้งผู้เช่ากับแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)[และกําหนดว่าผู้ใช้จะยินยอมให้แอปพลิเคชันอนุญาตอย่างไร](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- เข้าใจ[วิธีการการยินยอม](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)[และจัดการความยินยอมใน](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)แอปพลิเคชัน


