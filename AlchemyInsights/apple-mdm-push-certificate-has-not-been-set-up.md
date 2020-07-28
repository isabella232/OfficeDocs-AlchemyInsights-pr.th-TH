---
title: ไม่ได้ตั้งค่าใบรับรองการพุชของ Apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440008"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="dce18-102">ไม่ได้ตั้งค่าใบรับรองการพุชของ Apple MDM</span><span class="sxs-lookup"><span data-stu-id="dce18-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="dce18-103">ใบรับรองพุชของ Apple MDM (หรือที่เรียกอีกอย่างหนึ่งว่าใบรับรองบริการแจ้งเตือนแบบพุชของ Apple (APNS) ) ยังไม่ได้รับการกําหนดค่าสําหรับการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="dce18-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="dce18-104">หากไม่มีการกําหนดค่าใบรับรองการพุชของ Apple MDM คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ Mac OS ได้</span><span class="sxs-lookup"><span data-stu-id="dce18-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="dce18-105">หลังจากที่คุณเพิ่มใบรับรองไปยัง Intun</span><span class="sxs-lookup"><span data-stu-id="dce18-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="dce18-106">เลือก **"ฉันยอมรับ"**</span><span class="sxs-lookup"><span data-stu-id="dce18-106">Select **"I agree."**</span></span> <span data-ttu-id="dce18-107">เพื่อมอบสิทธิ์แก่ Microsoft ในการส่งข้อมูลไปยัง Apple</span><span class="sxs-lookup"><span data-stu-id="dce18-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="dce18-108">เลือก**ดาวน์โหลด CSR**ของคุณ</span><span class="sxs-lookup"><span data-stu-id="dce18-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="dce18-109">แฟ้มนี้ใช้เพื่อร้องขอใบรับรองความสัมพันธ์ความน่าเชื่อถือจากพอร์ทัลใบรับรองการพุชของ Apple</span><span class="sxs-lookup"><span data-stu-id="dce18-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="dce18-110">เลือก**สร้างใบรับรองการพุช MDM ของคุณเพื่อ**ไปที่พอร์ทัลใบรับรองการพุชของ Apple</span><span class="sxs-lookup"><span data-stu-id="dce18-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="dce18-111">ลงชื่อเข้าใช้ด้วย Apple ID ของบริษัทของคุณ แล้วเลือก**สร้างใบรับรอง**</span><span class="sxs-lookup"><span data-stu-id="dce18-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="dce18-112">เลือก**เลือก ไฟล์**เรียกดูไฟล์คําขอลงนามใบรับรอง แล้วเลือก**อัปโหลด**</span><span class="sxs-lookup"><span data-stu-id="dce18-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="dce18-113">บนหน้าการยืนยัน ให้เลือก**ดาวน์โหลด**เพื่อดาวน์โหลดไฟล์ใบรับรอง (.pem) และบันทึกไฟล์ภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="dce18-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="dce18-114">**หมายเหตุ**: ใบรับรองเชื่อมโยงกับ Apple ID ที่ใช้สร้าง</span><span class="sxs-lookup"><span data-stu-id="dce18-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="dce18-115">ใช้ Apple ID ของบริษัทสําหรับงานการจัดการ และตรวจสอบให้แน่ใจว่ากล่องจดหมายถูกตรวจสอบโดยบุคคลมากกว่าหนึ่งคนหรือโดยใช้รายชื่อการแจกจ่าย</span><span class="sxs-lookup"><span data-stu-id="dce18-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="dce18-116">ห้ามใช้ Apple ID ส่วนตัว</span><span class="sxs-lookup"><span data-stu-id="dce18-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="dce18-117">ใช้ Apple ID เดียวกันเพื่อต่ออายุใบรับรองการกดของ Apple ทุกๆ 12 เดือน</span><span class="sxs-lookup"><span data-stu-id="dce18-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="dce18-118">ป้อน Apple ID ที่ใช้สร้างใบรับรองการพุชของ Apple MDM ของคุณ</span><span class="sxs-lookup"><span data-stu-id="dce18-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="dce18-119">บันทึก ID นี้เป็นตัวเตือนสําหรับเวลาที่คุณต้องการต่ออายุใบรับรอง</span><span class="sxs-lookup"><span data-stu-id="dce18-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="dce18-120">ไปที่แฟ้มใบรับรอง (.pem) เลือก**เปิด**แล้วเลือก**อัปโหลด**</span><span class="sxs-lookup"><span data-stu-id="dce18-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="dce18-121">ด้วยใบรับรองแบบพุช Intun ณีสามารถลงทะเบียนและจัดการอุปกรณ์ Apple ได้</span><span class="sxs-lookup"><span data-stu-id="dce18-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>