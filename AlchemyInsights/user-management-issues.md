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
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971496"
---
# <a name="user-management-issues"></a>ปัญหาการจัดการผู้ใช้

**What happens to current assigned users to the application if I disable the property 'User assignment required' (set this property to No)?**

การปิดใช้งาน **การมอบหมายของผู้ใช้** ที่ต้องใช้จะไม่มีผลต่อผู้ใช้ที่ได้รับมอบหมายในปัจจุบัน การปิดใช้งานคุณสมบัตินี้จะอนุญาตให้ผู้ใช้ทั้งหมดเข้าถึงแอปพลิเคชันได้เท่านั้น ผู้ใช้ที่แสดงอยู่ในรายการและผู้ใช้ที่มอบหมายให้กลุ่มในแอปพลิเคชันจะยังคงใช้งานได้

- เมื่อต้องการจํากัดแอปของคุณเฉพาะชุดของผู้ใช้ ให้ดู -[จํากัดแอป Azure AD เป็นชุดของผู้ใช้ - เปิดใช้งานแพลตฟอร์มข้อมูลประจําตัวของ Microsoft | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)
- เมื่อต้องการกําหนดผู้ใช้และกลุ่มให้กับแอปพลิเคชันขององค์กรใน Azure Active Directory (Azure AD) ไม่ว่าจะจากภายในพอร์ทัล Azure หรือโดยใช้ PowerShell ให้ดู จัดการงานที่มอบหมายของผู้ใช้ของแอป[ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- เมื่อต้องการมอบสิทธิ์การสร้างและการจัดการแอปพลิเคชัน ให้ดู[มอบสิทธิ์ผู้ดูแลระบบการจัดการแอปพลิเคชัน - บัญชี Azure AD | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)
- **ซ่อนแอประดับองค์กรที่เฉพาะเจาะจง** จากผู้ใช้ - ใช้ขั้นตอนต่อไปนี้เพื่อซ่อนแอปMicrosoft 365ทั้งหมดจากแผง **MyApps** แอปจะยังคงมองเห็นได้ในพอร์ทัลOffice 365ของคุณ

 1. ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบส่วนกลางของไดเรกทอรีของคุณ 
 2. เลือก **Azure Active Directory** 
 3. เลือกผู้ใช้ 
 4. เลือก **การตั้งค่า** ผู้ใช้ 
 5. ภายใต้ **แอปพลิเคชัน** ขององค์กร **ให้คลิก จัดการวิธีเปิดใช้และดูแอปพลิเคชันของผู้ใช้** 
 6. **For Users can only see Office 365 apps in the Office 365 portal**, click **Yes**. 
 7. คลิก **บันทึก** 
 8. For more details, see [Hide an Enterprise application from user's experience in Azure AD | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- ถ้าคุณเสนอแอปซอฟต์แวร์เป็นบริการ (SaaS) ให้กับหลายองค์กร คุณสามารถกําหนดค่าแอปให้ยอมรับการลงชื่อเข้าใช้จากผู้เช่า Azure Active Directory (Azure AD) ใดก็ได้ การกําหนดค่านี้จะเรียกว่า "การกําหนดให้แอปพลิเคชันของคุณมีหลายผู้เช่า" ผู้ใช้ในผู้เช่า Azure AD จะสามารถลงชื่อเข้าใช้แอปของคุณหลังจากยินยอมใช้บัญชีของพวกเขากับแอปของคุณ For more information, see [Build apps that sign in Azure AD users - แพลตฟอร์มข้อมูลประจําตัวของ Microsoft | เอกสาร Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)

- **ผู้ใช้จะสามารถเข้าถึงแอปพลิเคชันเมื่อถูกมอบหมายไปยังแอปพลิเคชันได้อย่างไร**

แอปแต่ละแอปในใบแอปพลิเคชัน Enterprise จะมีลิงก์เพื่อให้ผู้ใช้เข้าถึงได้ ผู้ใช้ยังสามารถเข้าถึงแอปผ่านพอร์ทัล **แอป** ของฉัน ด้วยวิธีง่ายๆ

- **ต้องการทราบแอปพลิเคชันและชนิดของแอปพลิเคชันที่ถูกใช้โดยผู้ใช้หรือไม่**

คุณสามารถดาวน์โหลดรายงานการลงชื่อเข้าใช้ในช่วง 30 วันที่ผ่านมาจาก **portal.azure.com > Azure Active Directory>ลงชื่อเข้าใช้>ดาวน์โหลดรายงาน**

- เรียนรู้วิธีการให้[ความยินยอมของผู้ดูแลระบบทั้งผู้เช่ากับแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)[และ กําหนดค่าวิธีที่ผู้ใช้ยินยอมให้แอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- เข้าใจว่า[การยินยอมมีวิธีการ](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)[อย่างไรและจัดการความยินยอมต่อ](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)แอปพลิเคชัน


