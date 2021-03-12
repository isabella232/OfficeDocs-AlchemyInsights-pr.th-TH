---
title: กําหนดค่าการแจ้งเตือนการกักกันที่ส่งให้กับผู้ใช้
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 3e3e350f74b19420155c29cb282f065e7db6d4d7
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747939"
---
# <a name="configure-quarantine-notifications-sent-to-users"></a><span data-ttu-id="511e0-102">กําหนดค่าการแจ้งเตือนการกักกันที่ส่งให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="511e0-102">Configure quarantine notifications sent to users</span></span>

<span data-ttu-id="511e0-103">เมื่อต้องการส่งการแจ้งเตือนไปยังผู้ใช้ของคุณเกี่ยวกับสิ่งที่อยู่ในการกักกัน:</span><span class="sxs-lookup"><span data-stu-id="511e0-103">To send notifications to your users about what's in quarantine:</span></span>

1. <span data-ttu-id="511e0-104">ในศูนย์การจัดการ ให้นําทาง **ไปยังศูนย์การจัดการ**  >  **ตัวกรอง**  >    >  **สแปมใน** Exchange Protection</span><span class="sxs-lookup"><span data-stu-id="511e0-104">In the admin center, navigate to **admin centers** > **Exchange** > **Protection** > **spam filter**.</span></span>
2. <span data-ttu-id="511e0-105">เลือกนโยบายตัวกรองสแปมที่คุณต้องการเปิดการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="511e0-105">Select the spam filter policy for which you want to turn on notifications.</span></span>
3. <span data-ttu-id="511e0-106">ในบานหน้าต่างด้านขวา ให้เลือกลิงก์ **กําหนดค่าการแจ้งเตือนสแปมผู้ใช้** ปลายทาง</span><span class="sxs-lookup"><span data-stu-id="511e0-106">In the right pane, choose the **Configure End-user spam notifications** link.</span></span>
4. <span data-ttu-id="511e0-107">ในกล่องโต้ตอบถัดไป ให้เลือก **เปิดใช้งานการแจ้งเตือนสแปมผู้ใช้** ปลายทาง</span><span class="sxs-lookup"><span data-stu-id="511e0-107">In the next dialog box, choose **Enable end-user spam notifications**.</span></span> <span data-ttu-id="511e0-108">เลือกเพื่อเปิดใช้งานการแจ้งเตือนสแปมของนโยบายนี้</span><span class="sxs-lookup"><span data-stu-id="511e0-108">Choose to enable spam notifications for this policy.</span></span>
5. <span data-ttu-id="511e0-109">ใน **การแจ้งเตือนสแปมผู้ใช้ปลายทางทุกๆ (วัน)** ให้ระบุความถี่ในการส่งการแจ้งเตือนสแปมผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="511e0-109">In **Send end-user spam notifications every (days)**, specify how often to send user spam notifications.</span></span> <span data-ttu-id="511e0-110">ค่าเริ่มต้นคือ 3 วัน</span><span class="sxs-lookup"><span data-stu-id="511e0-110">The default is 3 days.</span></span> <span data-ttu-id="511e0-111">คุณสามารถระบุระหว่าง 1 และ 15 วัน</span><span class="sxs-lookup"><span data-stu-id="511e0-111">You can specify between 1 and 15 days.</span></span> <span data-ttu-id="511e0-112">ตัวอย่างเช่น ถ้าคุณระบุ 7 วัน การแจ้งให้ทราบจะมีรายการของข้อความทั้งหมดที่มีไว้ของผู้ใช้รายนั้นภายใน 7 วันที่ผ่านมาซึ่งถูกส่งไปยังการกักกันสแปมแทน</span><span class="sxs-lookup"><span data-stu-id="511e0-112">If you specify 7 days, for example, the notification will include a list of all messages intended for that user within the past 7 days that were sent to the spam quarantine instead.</span></span>
6. <span data-ttu-id="511e0-113">ในภาษา **การแจ้งเตือน** ให้เลือกภาษาที่จะเขียนการแจ้งเตือนสแปมผู้ใช้ของนโยบายนี้</span><span class="sxs-lookup"><span data-stu-id="511e0-113">In **Notification language** choose the language in which to write user spam notifications for this policy.</span></span>
7. <span data-ttu-id="511e0-114">เลือกบันทึก</span><span class="sxs-lookup"><span data-stu-id="511e0-114">Choose **Save**.</span></span>
