---
title: ส่งข้อความอีเมลด้วยการให้ ID ข้อความเครือข่าย
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
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695379"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="2ad24-102">ส่งข้อความอีเมลด้วยการให้ ID ข้อความเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="2ad24-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="2ad24-103">ใน **แถบปลิว** การส่งใหม่ **ให้เลือกอีเมล\*\*\*\*และ ID ข้อความ** เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="2ad24-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="2ad24-104">ให้ปฏิบัติตามขั้นตอนเหล่านี้เพื่อค้นหา ID ข้อความของข้อความอีเมลใน Outlook:</span><span class="sxs-lookup"><span data-stu-id="2ad24-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="2ad24-105">ดับเบิลคลิกที่ข้อความอีเมลเพื่อเปิด</span><span class="sxs-lookup"><span data-stu-id="2ad24-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="2ad24-106">**เลือก**  >  **คุณสมบัติ** ไฟล์</span><span class="sxs-lookup"><span data-stu-id="2ad24-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="2ad24-107">เปิด Notepad หรือเอกสาร Word เปล่า แล้วคัดลอกและวางเนื้อหาที่พบในกล่อง **ส่วนหัวอินเทอร์เน็ต** ลงในเอกสารที่เปิดอยู่เพื่อให้มองเห็นได้ดียิ่งขึ้น</span><span class="sxs-lookup"><span data-stu-id="2ad24-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="2ad24-108">ค้นหาเขตข้อมูล **X-MS-Exchange-Organization-Network-Message-Id**</span><span class="sxs-lookup"><span data-stu-id="2ad24-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="2ad24-109">ค่าหลังจาก **:** คือ ID ที่คุณต้องการส่ง</span><span class="sxs-lookup"><span data-stu-id="2ad24-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="2ad24-110">**ภายใต้ ผู้รับ** ถ้าอีเมลอยู่ในโฟลเดอร์อีเมลขยะของผู้รับอีเมลนี้ทั้งหมด ให้เลือก **เลือก** ทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="2ad24-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="2ad24-111">ถ้าไม่ ให้เลือกเฉพาะผู้ใช้ที่รายงานปัญหา</span><span class="sxs-lookup"><span data-stu-id="2ad24-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="2ad24-112">ภายใต้ **เหตุผล** ในการส่ง ถ้าคุณเลือกควรถูกบล็อก ให้ระบุว่าข้อความควรถูกบล็อกเป็น **สแปม** ฟิชชิ่ง หรือมัลแวร์ จากนั้นเลือกส่ง</span><span class="sxs-lookup"><span data-stu-id="2ad24-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="2ad24-113">เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดูวิธีการส่งสแปมที่น่าสงสัย, phish, URL และไฟล์ไปยัง Microsoft เพื่อสแกน](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="2ad24-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
