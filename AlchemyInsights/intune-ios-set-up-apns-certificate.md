---
title: Intun1 iOS ตั้งค่าใบรับรอง APNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 66590b8a063e74e80bbe3e1e497c596d63a54ece
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824058"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="f2c47-102">Intun1 iOS ตั้งค่าใบรับรอง APNS</span><span class="sxs-lookup"><span data-stu-id="f2c47-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="f2c47-103">ใบรับรอง Apple MDM Push (หรือที่เรียกว่าใบรับรอง Apple Push Notification Service (APNS) ยังไม่ได้กําหนดค่าในการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2c47-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="f2c47-104">ถ้าไม่มีใบรับรองแบบพุชของ Apple MDM ที่กําหนดค่าไว้ คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ MacOS ได้</span><span class="sxs-lookup"><span data-stu-id="f2c47-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="f2c47-105">หลังจากที่คุณเพิ่มใบรับรองไปยัง Intun1 ผู้ใช้ของคุณสามารถติดตั้งแอป Company Portal เพื่อลงทะเบียนอุปกรณ์ iOS ของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="f2c47-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="f2c47-106">โปรดดูเนื้อหาบนลิงก์ต่อไปนี้เพื่อไปยังคู่มือทีละขั้นตอนในการเพิ่มใบรับรอง APNS ลงในผู้เช่า Intunte ของคุณ</span><span class="sxs-lookup"><span data-stu-id="f2c47-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="f2c47-107">รับใบรับรองแบบพุช MDM ของ Apple</span><span class="sxs-lookup"><span data-stu-id="f2c47-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="f2c47-108">ถ้าคุณมีปัญหากับใบรับรองการแจ้งเตือนแบบพุช (APN) ของ Apple ให้อ้างอิงโพสต์ในบล็อกนี้: Intun1 และใบรับรอง [APN: FAQ และปัญหาทั่วไป](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="f2c47-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
