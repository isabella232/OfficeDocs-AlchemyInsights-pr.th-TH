---
title: แก้ไขปัญหารหัสข้อผิดพลาดการรับรองความถูกต้องของ Azure AD และการอนุญาต (AADSTS)
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
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037841"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="cdced-102">แก้ไขปัญหารหัสข้อผิดพลาดการรับรองความถูกต้องของ Azure AD และการอนุญาต (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="cdced-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="cdced-103">เมื่อต้องการแก้ไขการรับรองความถูกต้อง AAD และรหัสข้อผิดพลาดการรับรองความถูกต้อง (AADSTS) ให้ปฏิบัติตามขั้นตอนที่แนะนาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="cdced-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="cdced-104">**การจัดการรหัสข้อผิดพลาดในแอปพลิเคชันของคุณ**</span><span class="sxs-lookup"><span data-stu-id="cdced-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="cdced-105">ข้อ **กําหนด OAuth2.0** ให้แนวทางเกี่ยวกับวิธีการ https://tools.ietf.org/html/rfc6749#section-5.2 จัดการกับข้อผิดพลาดระหว่างการรับรองความถูกต้องโดยใช้ส่วนข้อผิดพลาดของการตอบกลับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="cdced-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="cdced-106">**ข้อผิดพลาด**: สตริงรหัสข้อผิดพลาดที่สามารถใช้เพื่อจัดประเภทข้อผิดพลาดที่เกิดขึ้น และควรใช้เพื่อตอบสนองต่อข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="cdced-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="cdced-107">เขตข้อมูล **ข้อผิดพลาด** มีค่าที่เป็นไปได้หลายค่า - ตรวจทานลิงก์คู่มือโพรโทคอลและข้อเฉพาะเจาะจง OAuth 2.0 เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดที่เฉพาะเจาะจงและวิธีการตอบสนองต่อข้อผิดพลาดเหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="cdced-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="cdced-108">นี่คือตัวอย่างการตอบสนองข้อผิดพลาด:</span><span class="sxs-lookup"><span data-stu-id="cdced-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="cdced-109">**ค้นหาข้อมูลรหัสข้อผิดพลาดปัจจุบัน**</span><span class="sxs-lookup"><span data-stu-id="cdced-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="cdced-110">รหัสข้อผิดพลาดและข้อความอาจเปลี่ยนแปลงได้</span><span class="sxs-lookup"><span data-stu-id="cdced-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="cdced-111">ดูข้อมูลล่าสุดที่หน้าเพื่อค้นหา https://login.microsoftonline.com/error รายละเอียดข้อผิดพลาด AADSTS การแก้ไข และการแก้ไขปัญหาชั่วคราวที่แนะน</span><span class="sxs-lookup"><span data-stu-id="cdced-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="cdced-112">คุณยังสามารถค้นหาและแก้ไขปัญหารหัสข้อผิดพลาด[AADSTS ที่แสดง](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)อยู่ในบทความ การรับรองความถูกต้อง[Azure AD และรหัสข้อผิดพลาดการอนุญาต](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="cdced-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="cdced-113">**ดูวิธีใช้**</span><span class="sxs-lookup"><span data-stu-id="cdced-113">**Get Help**</span></span>

- <span data-ttu-id="cdced-114">[ตัวเลือกการสนับสนุนและวิธีใช้](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) ของนักพัฒนา - ถ้าคุณต้องการคําตอบของคําถามหรือความช่วยเหลือในการแก้ไขปัญหาที่ไม่ครอบคลุมอยู่ในเอกสารประกอบของเรา อาจถึงเวลาที่จะติดต่อผู้เชี่ยวชาญเพื่อขอความช่วยเหลือ</span><span class="sxs-lookup"><span data-stu-id="cdced-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="cdced-115">บทความนี้มีคําแนะนเกี่ยวกับการรับคําตอบของคําถามของคุณเมื่อคุณพัฒนาแอปที่รวมเข้ากับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="cdced-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








