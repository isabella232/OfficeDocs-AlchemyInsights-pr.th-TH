---
title: ตั้งค่าใบรับรอง APNS ของ iOS Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 027e1e0fa3b625fa0f619bc6d74844f6ec5be769
ms.sourcegitcommit: 75346a972c2174248de3bb55a19d714cee43c1cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/09/2020
ms.locfileid: "43211433"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="aea8c-102">ตั้งค่าใบรับรอง APNS ของ iOS Intune</span><span class="sxs-lookup"><span data-stu-id="aea8c-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="aea8c-103">ใบรับรอง Apple MDM Push (หรือที่เรียกว่าใบรับรองบริการแจ้งเตือนแบบพุช (APNS) ของ Apple) ยังไม่ได้รับการกําหนดค่าในการสมัครใช้งานของคุณ</span><span class="sxs-lookup"><span data-stu-id="aea8c-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="aea8c-104">หากไม่มีการกําหนดค่าใบรับรอง Apple MDM Push คุณจะไม่สามารถลงทะเบียนและจัดการอุปกรณ์ iOS และ MacOS ได้</span><span class="sxs-lookup"><span data-stu-id="aea8c-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="aea8c-105">หลังจากที่คุณเพิ่มใบรับรองไปยัง Intune ผู้ใช้ของคุณสามารถติดตั้งแอปพอร์ทัลของบริษัทเพื่อลงทะเบียนอุปกรณ์ iOS ของตนได้</span><span class="sxs-lookup"><span data-stu-id="aea8c-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="aea8c-106">สําหรับคําแนะนําทีละขั้นตอนในการเพิ่มใบรับรอง APNS กับผู้เช่า Intune ของคุณ โปรดตรวจทานเนื้อหาในการเชื่อมโยงต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="aea8c-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="aea8c-107">รับใบรับรองการผลักดัน MDM ของ Apple</span><span class="sxs-lookup"><span data-stu-id="aea8c-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="aea8c-108">หากคุณมีปัญหากับใบรับรองการแจ้งเตือนแบบพุชของ Apple (APNs) โปรดดูโพสต์บล็อกนี้: [Intune และใบรับรอง APNs: คําถามที่ถามบ่อยและปัญหาทั่วไป](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="aea8c-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
