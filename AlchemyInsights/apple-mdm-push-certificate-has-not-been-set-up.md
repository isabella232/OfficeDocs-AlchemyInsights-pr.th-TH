---
title: ยังไม่ได้ตั้งค่าใบรับรองแบบพุชของ Apple MDM ของ Apple
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716876"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="3ec9d-102">ยังไม่ได้ตั้งค่าใบรับรองแบบพุชของ Apple MDM ของ Apple</span><span class="sxs-lookup"><span data-stu-id="3ec9d-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="3ec9d-103">ใบรับรองแบบพุชของ Apple MDM (หรือที่เรียกว่าใบรับรองบริการการแจ้งเตือนแบบพุชของ Apple (APN)) ยังไม่ได้รับการกำหนดค่าสำหรับการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="3ec9d-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="3ec9d-104">ถ้าไม่มีการกำหนดค่าใบรับรองแบบผลักข้อมูลของ Apple MDM คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ Mac OS ได้</span><span class="sxs-lookup"><span data-stu-id="3ec9d-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="3ec9d-105">หลังจากที่คุณเพิ่มใบรับรองไปยัง Intune แล้วผู้ใช้สามารถติดตั้งแอป Portal ของบริษัทเพื่อลงทะเบียนอุปกรณ์ iOS ของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="3ec9d-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="3ec9d-106">เลือก **"ฉันยอมรับ"**</span><span class="sxs-lookup"><span data-stu-id="3ec9d-106">Select **"I agree."**</span></span> <span data-ttu-id="3ec9d-107">เมื่อต้องการให้สิทธิ์ Microsoft ส่งข้อมูลไปยัง Apple</span><span class="sxs-lookup"><span data-stu-id="3ec9d-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="3ec9d-108">เลือก **ดาวน์โหลด CSR ของคุณ** การร้องขอการเซ็นชื่อใบรับรอง Intune ของคุณจำเป็นต้องใช้ในการสร้างใบรับรองแบบพุชของ Apple MDM</span><span class="sxs-lookup"><span data-stu-id="3ec9d-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="3ec9d-109">ไฟล์จะถูกใช้เพื่อร้องขอใบรับรองความสัมพันธ์ที่เชื่อถือจากพอร์ทัลใบรับรองแบบพุชของ Apple</span><span class="sxs-lookup"><span data-stu-id="3ec9d-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="3ec9d-110">เลือก **สร้างใบรับรองแบบผลักข้อมูล MDM ของคุณ** เพื่อไปที่พอร์ทัลใบรับรองแบบพุชของ Apple</span><span class="sxs-lookup"><span data-stu-id="3ec9d-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="3ec9d-111">ลงชื่อเข้าใช้ด้วย Apple ID ของบริษัทของคุณจากนั้นเลือก**สร้างใบรับรอง**</span><span class="sxs-lookup"><span data-stu-id="3ec9d-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="3ec9d-112">เลือก**เลือกไฟล์**เรียกดูไฟล์คำขอการเซ็นชื่อใบรับรองจากนั้นเลือก**อัปโหลด**</span><span class="sxs-lookup"><span data-stu-id="3ec9d-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="3ec9d-113">บนหน้าการยืนยันให้เลือก **ดาวน์โหลด** เพื่อดาวน์โหลดไฟล์ใบรับรอง (pem) และบันทึกไฟล์ภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="3ec9d-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="3ec9d-114">**หมายเหตุ**: ใบรับรองเชื่อมโยงกับ Apple ID ที่ใช้ในการสร้างใบรับรองนั้น</span><span class="sxs-lookup"><span data-stu-id="3ec9d-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="3ec9d-115">เพื่อเป็นแนวทางปฏิบัติที่ดีที่สุดให้ใช้ Apple ID สำหรับงานการจัดการและตรวจสอบให้แน่ใจว่ากล่องจดหมายได้รับการตรวจสอบโดยผู้ใช้มากกว่าหนึ่งคนหรือโดยใช้รายชื่อการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="3ec9d-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="3ec9d-116">อย่าใช้ Apple ID ส่วนบุคคล</span><span class="sxs-lookup"><span data-stu-id="3ec9d-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="3ec9d-117">ใช้ Apple ID เดียวกันเพื่อต่ออายุใบรับรองแบบพุชของ Apple ทุกๆ12เดือน</span><span class="sxs-lookup"><span data-stu-id="3ec9d-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="3ec9d-118">ใส่ Apple ID ที่ใช้ในการสร้างใบรับรองแบบพุชของ Apple MDM ของ Apple</span><span class="sxs-lookup"><span data-stu-id="3ec9d-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="3ec9d-119">บันทึก ID นี้เป็นตัวเตือนเมื่อคุณต้องการต่ออายุใบรับรอง</span><span class="sxs-lookup"><span data-stu-id="3ec9d-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="3ec9d-120">ไปที่ไฟล์ใบรับรอง (pem) เลือก**เปิด**แล้วเลือก**อัปโหลด**</span><span class="sxs-lookup"><span data-stu-id="3ec9d-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="3ec9d-121">ด้วยใบรับรองแบบพุช Intune สามารถลงทะเบียนและจัดการอุปกรณ์ Apple ได้</span><span class="sxs-lookup"><span data-stu-id="3ec9d-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>