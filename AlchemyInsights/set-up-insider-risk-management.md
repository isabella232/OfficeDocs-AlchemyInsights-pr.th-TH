---
title: ตั้งค่าการจัดการความเสี่ยงของ insider
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002284"
- "4405"
ms.openlocfilehash: 3cde8bb419d79506e101cd75fde6fcb69aa2441c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800987"
---
# <a name="set-up-insider-risk-management"></a><span data-ttu-id="1be2c-102">ตั้งค่าการจัดการความเสี่ยงของ insider</span><span class="sxs-lookup"><span data-stu-id="1be2c-102">Set up insider risk management</span></span>

<span data-ttu-id="1be2c-103">ใช้นโยบายการจัดการความเสี่ยงของ insider เพื่อระบุกิจกรรมที่มีความเสี่ยงและเครื่องมือการจัดการเพื่อดำเนินการแจ้งเตือนเกี่ยวกับความเสี่ยงในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="1be2c-103">Use insider risk management policies to identify risky activities and management tools to take action on risk alerts in your organization.</span></span> <span data-ttu-id="1be2c-104">ก่อนที่คุณจะเริ่มต้นใช้งานการจัดการความเสี่ยงของ insider คุณควรยืนยันการสมัครใช้งาน **Microsoft ๓๖๕**ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1be2c-104">Before you get started with insider risk management, you should confirm your **Microsoft 365 subscription**.</span></span> <span data-ttu-id="1be2c-105">เมื่อต้องการเข้าถึงและใช้การจัดการความเสี่ยงของ insider องค์กรของคุณจะ **ต้อง** มีหนึ่งในการสมัครใช้งานต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="1be2c-105">To access and use insider risk management, your organization **must** have one of the following subscriptions:</span></span>

- <span data-ttu-id="1be2c-106">การสมัครใช้งาน**Microsoft ๓๖๕ E5**</span><span class="sxs-lookup"><span data-stu-id="1be2c-106">**Microsoft 365 E5** subscription.</span></span>

- <span data-ttu-id="1be2c-107">การสมัครใช้งาน**microsoft ๓๖๕ E3**ที่มี add-on การปฏิบัติตามข้อบังคับของ microsoft E5</span><span class="sxs-lookup"><span data-stu-id="1be2c-107">**Microsoft 365 E3** subscription with the Microsoft E5 compliance add-on.</span></span>

<span data-ttu-id="1be2c-108">ถ้าคุณไม่มีแผน **Microsoft ๓๖๕ E5** ที่มีอยู่และต้องการทดลองใช้งานการจัดการความเสี่ยงของ insider คุณสามารถเพิ่ม Microsoft ๓๖๕ลงในการสมัครใช้งานที่มีอยู่ของคุณหรือลงทะเบียนสำหรับเวอร์ชันทดลองใช้ของ Microsoft ๓๖๕ Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="1be2c-108">If you don't have an existing **Microsoft 365 E5** plan and want to try insider risk management, you can add Microsoft 365 to your existing subscription or Sign up for a trial of Microsoft 365 Enterprise E5.</span></span>

<span data-ttu-id="1be2c-109">ขั้นตอนพื้นฐานสำหรับการใช้การจัดการความเสี่ยงของ Insider มีดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="1be2c-109">The basic steps for using Insider Risk Management include:</span></span>

1. <span data-ttu-id="1be2c-110">เปิดใช้งานสิทธิ์สำหรับการจัดการความเสี่ยงของ insider</span><span class="sxs-lookup"><span data-stu-id="1be2c-110">Enable permissions for insider risk management.</span></span>

2. <span data-ttu-id="1be2c-111">เปิดใช้งานบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="1be2c-111">Enable the audit log.</span></span>

3. <span data-ttu-id="1be2c-112">กำหนดค่าข้อกำหนดเบื้องต้นสำหรับเทมเพลต (ไม่จำเป็น)</span><span class="sxs-lookup"><span data-stu-id="1be2c-112">Configure prerequisites for template (optional).</span></span>

4. <span data-ttu-id="1be2c-113">กำหนดค่าการตั้งค่าความเสี่ยงของ insider</span><span class="sxs-lookup"><span data-stu-id="1be2c-113">Configure insider risk settings.</span></span>

5. <span data-ttu-id="1be2c-114">สร้างนโยบายการจัดการความเสี่ยงของ insider</span><span class="sxs-lookup"><span data-stu-id="1be2c-114">Create an insider risk management policy.</span></span>

<span data-ttu-id="1be2c-115">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีที่นโยบายความเสี่ยงของ insider สามารถช่วยคุณจัดการความเสี่ยงในองค์กรของคุณให้ดูที่[การจัดการความเสี่ยงของ insider ใน Microsoft ๓๖๕](https://go.microsoft.com/fwlink/?linkid=2123907)</span><span class="sxs-lookup"><span data-stu-id="1be2c-115">For more information about how insider risk polices can help you manage risk in your Organization, see [Insider risk management in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2123907).</span></span>
