---
title: คืนค่าฟอร์มที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809494"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="1b770-102">คืนค่าฟอร์มที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="1b770-102">Restore a deleted form</span></span>

<span data-ttu-id="1b770-103">ถ้าคุณลบฟอร์มใน Microsoft Forms โดยบังเอิญ คุณสามารถกู้คืนได้</span><span class="sxs-lookup"><span data-stu-id="1b770-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="1b770-104">ลงชื่อเข้าใช้ Microsoft Forms ในฐานะเจ้าของฟอร์มที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="1b770-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="1b770-105">เลือก **ถัง** รีไซเคิล จากนั้นเลือกฟอร์มที่คุณต้องการกู้คืน **และเลือก** คืนค่า</span><span class="sxs-lookup"><span data-stu-id="1b770-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="1b770-106">เมื่อคืนค่าแล้ว ให้เลือก **ลูกศร กลับไปยังหน้า ฟอร์ม** ของฉัน</span><span class="sxs-lookup"><span data-stu-id="1b770-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="1b770-107">เฉพาะเจ้าของฟอร์มเท่านั้นที่สามารถกู้คืนได้</span><span class="sxs-lookup"><span data-stu-id="1b770-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="1b770-108">ถ้าบัญชีผู้ใช้ของเจ้าของฟอร์มถูกปิดใช้งานหรือถูกเอาออกจากผู้เช่า เฉพาะผู้ดูแลระบบส่วนกลางเท่านั้นที่สามารถกู้คืนฟอร์มได้</span><span class="sxs-lookup"><span data-stu-id="1b770-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="1b770-109">ผู้ดูแลระบบส่วนกลางต้องมีสิทธิ์การใช้งาน Forms เพื่อคืนค่า</span><span class="sxs-lookup"><span data-stu-id="1b770-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="1b770-110">เฉพาะฟอร์มที่สร้างขึ้นภายใน 30 วันของบัญชีผู้ใช้ที่ถูกปิดใช้งานหรือถูกเอาออกจากผู้เช่าเท่านั้นที่สามารถคืนค่าได้</span><span class="sxs-lookup"><span data-stu-id="1b770-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="1b770-111">ถ้าคุณเป็นผู้ดูแลระบบส่วนกลางของผู้เช่า และคุณต้องการกู้คืนฟอร์มจากบัญชีที่ถูกลบหรือถูกปิดใช้งาน ให้แทนที่ [ที่อยู่อีเมล] ด้วยที่อยู่อีเมลของผู้ใช้ที่ถูกลบหรือถูกปิดใช้งานใน URL ต่อไปนี้: **https://forms.office.com/Pages/delegatepage.aspx?originalowner= [ที่อยู่อีเมล]** ตัวอย่างเช่น ถ้าที่อยู่อีเมลของคุณคือ johndoe@contoso.com URL **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** จะเป็น:</span><span class="sxs-lookup"><span data-stu-id="1b770-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="1b770-112">เมื่อคุณมีสิทธิ์เข้าถึงฟอร์มที่ถูกลบของผู้ใช้ ให้เลือกฟอร์มที่คุณต้องการย้าย แล้วเลือก การเคลื่อนย้าย **ฟอร์ม**  >  เพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="1b770-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="1b770-113">ถ้าคุณต้องการกู้คืนฟอร์มที่ถูกลบและผู้ใช้ถูกเอาออกจากองค์กร ผู้ดูแลระบบส่วนกลางสามารถเลือกที่จะกู้คืนผู้ใช้ ตั้งค่ารหัสผ่านใหม่ให้กับผู้ใช้รายนั้น แล้วเมื่อเข้าสู่ระบบในฐานะผู้ใช้รายนั้น ให้เข้าถึงฟอร์มเพื่อย้ายไปยังผู้ใช้อื่นที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="1b770-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 