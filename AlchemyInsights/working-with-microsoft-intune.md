---
title: การทำงานกับ Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/17/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "862"
- "670000"
ms.openlocfilehash: 8d900198114703fb31157fa9724f4f9711b7b8c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796379"
---
# <a name="working-with-microsoft-intune"></a><span data-ttu-id="f1369-102">การทำงานกับ Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f1369-102">Working with Microsoft Intune</span></span>

<span data-ttu-id="f1369-103">ดูเหมือนว่าคุณกำลังถามเกี่ยวกับ Intune</span><span class="sxs-lookup"><span data-stu-id="f1369-103">It looks like you're asking about Intune.</span></span> <span data-ttu-id="f1369-104">เราอาจจะช่วยเหลือคุณในการตอบคำถามที่ชัดเจนยิ่งขึ้นถ้าคุณบรรยายคำถามของคุณกับประโยคสั้นๆหนึ่งหรือสองประโยคที่อธิบายปัญหาของคุณรวมถึงข้อผิดพลาดฟีเจอร์ที่คุณกำลังใช้อยู่และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="f1369-104">We might be able to help with a more precise answer if you rephrase your question with one or two short sentences that describe your issue, including errors, features you’re using, and so on.</span></span> <span data-ttu-id="f1369-105">ในระหว่างนี้ต่อไปนี้เป็นข้อมูลบางอย่างเกี่ยวกับ Intune</span><span class="sxs-lookup"><span data-stu-id="f1369-105">In the meantime, here is some information about Intune.</span></span>

- [<span data-ttu-id="f1369-106">Intune คืออะไร</span><span class="sxs-lookup"><span data-stu-id="f1369-106">What is Intune?</span></span>](https://docs.microsoft.com/intune/what-is-intune)
- [<span data-ttu-id="f1369-107">วิธีการลงทะเบียนสำหรับเวอร์ชันทดลองใช้ของ Intune</span><span class="sxs-lookup"><span data-stu-id="f1369-107">How to sign up for Intune trial?</span></span>](https://docs.microsoft.com/intune/free-trial-sign-up)
- [<span data-ttu-id="f1369-108">ตั้งค่า Intune เป็นครั้งแรกใช่หรือไม่</span><span class="sxs-lookup"><span data-stu-id="f1369-108">Setup Intune for first time?</span></span>](https://docs.microsoft.com/intune/setup-steps)
- [<span data-ttu-id="f1369-109">การลงทะเบียนอุปกรณ์คืออะไร</span><span class="sxs-lookup"><span data-stu-id="f1369-109">What is device enrollment?</span></span>](https://docs.microsoft.com/intune/device-enrollment)
- [<span data-ttu-id="f1369-110">ข้อมูลพื้นฐานเกี่ยวกับการจัดการอุปกรณ์</span><span class="sxs-lookup"><span data-stu-id="f1369-110">Device Management Fundamentals</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/)

<span data-ttu-id="f1369-111">สำหรับรายละเอียดเกี่ยวกับการแก้ไขปัญหาใน Intune ให้ดูดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="f1369-111">For details about troubleshooting issues in Intune, see the following:</span></span>

- <span data-ttu-id="f1369-112">เมื่อต้องการวินิจฉัยและแก้ไขปัญหาความล้มเหลวทั่วไปให้ดูที่[พอร์ทัลการแก้ไขปัญหาของ Intune](https://aka.ms/intunetroubleshooting)</span><span class="sxs-lookup"><span data-stu-id="f1369-112">To diagnose and resolve common failures, see  [Intune Troubleshooting Portal](https://aka.ms/intunetroubleshooting).</span></span> <span data-ttu-id="f1369-113">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ใช้พอร์ทัลการแก้ไขปัญหาเพื่อช่วยผู้ใช้ที่บริษัทของคุณ](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="f1369-113">For more information, see [Use the troubleshooting portal to help users at your company](https://docs.microsoft.com/intune/help-desk-operators).</span></span>
- <span data-ttu-id="f1369-114">เมื่อต้องการค้นหาคำตอบและวิธีแก้ไขปัญหาทั่วไปให้ดูที่[Intune TechNet](https://aka.ms/intuneforums)</span><span class="sxs-lookup"><span data-stu-id="f1369-114">To find answers and solutions to common issues, see [Intune TechNet](https://aka.ms/intuneforums).</span></span>
- <span data-ttu-id="f1369-115">เมื่อต้องการดูสถานะของบริการของคุณให้ดูที่[สถานภาพบริการ](https://portal.office.com/AdminPortal/Home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="f1369-115">To view the status of your service, see [Service Health](https://portal.office.com/AdminPortal/Home#/servicehealth).</span></span>
- <span data-ttu-id="f1369-116">สำหรับการวางแผนวิธีการและข้อมูลการแก้ไขปัญหาให้ดูที่[เอกสารประกอบของ Intune](https://docs.microsoft.com/intune/)</span><span class="sxs-lookup"><span data-stu-id="f1369-116">For planning, how-to, and troubleshooting info, see the [Intune documentation](https://docs.microsoft.com/intune/).</span></span>