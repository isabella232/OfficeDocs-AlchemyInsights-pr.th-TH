---
title: การแจ้งเตือน AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037234"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="46d0f-102">การแจ้งเตือน AAD Connect</span><span class="sxs-lookup"><span data-stu-id="46d0f-102">Notification AAD Connect</span></span>

- <span data-ttu-id="46d0f-103">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการ</span><span class="sxs-lookup"><span data-stu-id="46d0f-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="46d0f-104">ผู้ดูแลระบบส่วนกลางมีสิทธิ์เข้าถึงได้ตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="46d0f-104">Global Admins have access by default.</span></span> <span data-ttu-id="46d0f-105">นอกจากนี้ คุณสามารถใช้การควบคุมการเข้าถึง [ตามบทบาทเพื่อมอบ](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) สิทธิ์การลงทะเบียนให้กับผู้สนับสนุน</span><span class="sxs-lookup"><span data-stu-id="46d0f-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="46d0f-106">ตรวจสอบให้แน่ใจว่าจุดสิ้นสุดที่กําหนดเปิดใช้งาน และไม่ถูกบล็อกเนื่องจากไฟร์วอลล์</span><span class="sxs-lookup"><span data-stu-id="46d0f-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="46d0f-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="46d0f-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="46d0f-108">การลงทะเบียนอาจล้มเหลวเนื่องจากการสื่อสารขาออกต้องผ่านการตรวจสอบ SSL โดยชั้นเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="46d0f-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="46d0f-109">ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบการตั้งค่าการแจ้งเตือนของ Azure AD Connect Health และตรวจสอบการตั้งค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="46d0f-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="46d0f-110">เมื่อต้องการเข้าใจวิธีกําหนดค่าการตั้งค่าการแจ้งเตือนการแจ้งเตือนของ Azure AD Connect Health ให้ดู [คู่มือ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)นี้</span><span class="sxs-lookup"><span data-stu-id="46d0f-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="46d0f-111">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับรายงานการซิงค์ AAD Connect Health และวิธีดาวน์โหลด ให้ดู [รายงานการซิงโครไนซ์ระดับ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)วัตถุ</span><span class="sxs-lookup"><span data-stu-id="46d0f-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="46d0f-112">เมื่อต้องการแก้ไขปัญหาการแจ้งเตือนสถานภาพของ AAD Connect ให้ปฏิบัติตามคู่มือการแก้ไขปัญหาเกี่ยวกับการแจ้งเตือนความสมบูรณ์ของข้อมูล [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) และถามบ่อย ให้ดูข้อถามการติดตั้ง [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="46d0f-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
