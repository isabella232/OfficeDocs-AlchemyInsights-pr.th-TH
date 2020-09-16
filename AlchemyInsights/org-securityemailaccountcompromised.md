---
title: ๔๒๓การรักษาความปลอดภัยขององค์กร-EmailAccountCompromised
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: 423
ms.assetid: f93a7a44-0cdf-4387-b428-53e1a48f63ce
ms.openlocfilehash: 94d8eec4f10e3df5ccdd891b7ae12c97bbb4d594
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724418"
---
# <a name="compromised-email-accounts"></a><span data-ttu-id="7cb36-102">บัญชีผู้ใช้อีเมลที่ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="7cb36-102">Compromised email accounts</span></span>

<span data-ttu-id="7cb36-103">มีหลายขั้นตอนที่คุณสามารถดำเนินการเพื่อช่วยเพิ่มความปลอดภัยในองค์กรของคุณได้ดังนี้</span><span class="sxs-lookup"><span data-stu-id="7cb36-103">There are several steps you can take to help increase security in your organization:</span></span>

- <span data-ttu-id="7cb36-104">**เปิดใช้งานการรับรองความถูกต้องแบบหลายปัจจัย (MFA)**: ถ้าบัญชีผู้ใช้ถูกบุกรุกการตั้งค่ารหัสผ่านใหม่ตามด้วยการเปิดใช้งาน MFA เป็นวิธีที่ดีที่จะช่วยให้แน่ใจว่าจะไม่เกิดขึ้นอีก</span><span class="sxs-lookup"><span data-stu-id="7cb36-104">**Enable multi-factor authentication (MFA)**: If an account has been compromised, resetting the password followed by enabling MFA is a good way to help ensure it doesn't happen again.</span></span> <span data-ttu-id="7cb36-105">ถ้ามีการใช้บัญชีผู้ใช้ที่ถูกบุกรุกในการส่งสแปมอาจถูกบล็อกไม่ให้ส่งอีเมล (แม้ว่าคุณจะดำเนินการตามขั้นตอนในการรักษาความปลอดภัย)</span><span class="sxs-lookup"><span data-stu-id="7cb36-105">If the compromised account was used to send spam, it's probably blocked from sending email (even after you take steps to secure it).</span></span> <span data-ttu-id="7cb36-106">เมื่อต้องการเอาผู้ใช้ออกจากรายการบล็อกให้ดู[หัวข้อนี้](https://technet.microsoft.com/library/ms.exch.eac.actioncenter.aspx)</span><span class="sxs-lookup"><span data-stu-id="7cb36-106">To remove the user from the block list, see [this topic](https://technet.microsoft.com/library/ms.exch.eac.actioncenter.aspx).</span></span>

- <span data-ttu-id="7cb36-107">**เรียกใช้คะแนนความปลอดภัยของ Office ๓๖๕**: คะแนนที่ปลอดภัยการวิเคราะห์โดยละเอียดของการตั้งค่าความปลอดภัยในองค์กรของคุณและให้คำแนะนำสำหรับการทำให้มีความปลอดภัยมากขึ้น</span><span class="sxs-lookup"><span data-stu-id="7cb36-107">**Run Office 365 Secure Score**: Secure Score does a detailed analysis of the security settings in your organization and provides recommendations for making it more secure.</span></span>

- <span data-ttu-id="7cb36-108">**เปิดใช้งานการบันทึกการตรวจสอบของกล่องจดหมาย**: บันทึกการตรวจสอบของกล่องจดหมายจะทำให้ง่ายต่อการติดตามสิ่งที่เกิดขึ้นเมื่อบัญชีผู้ใช้ถูกบุกรุก</span><span class="sxs-lookup"><span data-stu-id="7cb36-108">**Enable mailbox audit logging**: Mailbox audit logging will make it easier to track what happened when a user account is compromised.</span></span>

<span data-ttu-id="7cb36-109">สำหรับข้อมูลเพิ่มเติมให้ดูที่[แผนการรักษาความปลอดภัยของ Microsoft ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/security-roadmap)</span><span class="sxs-lookup"><span data-stu-id="7cb36-109">For more information, see [Microsoft 365 security roadmap](https://docs.microsoft.com/microsoft-365/security/office-365-security/security-roadmap).</span></span>
