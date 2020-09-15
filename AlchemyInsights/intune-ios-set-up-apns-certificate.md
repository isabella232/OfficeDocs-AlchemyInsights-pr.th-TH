---
title: การตั้งค่าใบรับรอง APN iOS ของ Intune
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
- "9000654"
- "3543"
ms.openlocfilehash: f58405de018c916e08672022bb4f66292524b736
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667465"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="4cf0c-102">การตั้งค่าใบรับรอง APN iOS ของ Intune</span><span class="sxs-lookup"><span data-stu-id="4cf0c-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="4cf0c-103">ใบรับรองแบบพุชของ Apple MDM (หรือที่เรียกว่าใบรับรองบริการการแจ้งเตือนแบบพุชของ Apple (APN)) ไม่ได้ถูกกำหนดค่าในการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="4cf0c-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="4cf0c-104">ถ้าไม่มีการกำหนดค่าใบรับรองแบบผลักข้อมูลของ Apple MDM คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ MacOS ได้</span><span class="sxs-lookup"><span data-stu-id="4cf0c-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="4cf0c-105">หลังจากที่คุณเพิ่มใบรับรองไปยัง Intune แล้วผู้ใช้ของคุณสามารถติดตั้งแอป Portal ของบริษัทเพื่อลงทะเบียนอุปกรณ์ iOS ของพวกเขาได้</span><span class="sxs-lookup"><span data-stu-id="4cf0c-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="4cf0c-106">สำหรับคำแนะนำทีละขั้นตอนในการเพิ่มใบรับรอง APN ให้กับผู้เช่า Intune ของคุณโปรดตรวจทานเนื้อหาบนลิงก์ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="4cf0c-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="4cf0c-107">รับใบรับรองแบบพุชของ Apple MDM</span><span class="sxs-lookup"><span data-stu-id="4cf0c-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="4cf0c-108">ถ้าคุณกำลังมีปัญหาเกี่ยวกับใบรับรองการแจ้งเตือนแบบพุชของ Apple (Apn) อ้างอิงไปยังโพสต์ในบล็อกนี้: [Intune และใบรับรอง apn: คำถามที่ถามบ่อยและปัญหาทั่วไป](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="4cf0c-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
