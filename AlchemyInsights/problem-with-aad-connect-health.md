---
title: ปัญหากับ AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483122"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="e9682-102">ปัญหากับ AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="e9682-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="e9682-103">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ดําเนินการ</span><span class="sxs-lookup"><span data-stu-id="e9682-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="e9682-104">ผู้ดูแลระบบส่วนกลางมีสิทธิ์เข้าถึงได้ตามค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="e9682-104">Global Admins have access by default.</span></span> <span data-ttu-id="e9682-105">นอกจากนี้ คุณสามารถใช้การควบคุมการเข้าถึง [ตามบทบาทเพื่อมอบ](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) สิทธิ์การลงทะเบียนให้กับผู้สนับสนุน</span><span class="sxs-lookup"><span data-stu-id="e9682-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="e9682-106">ตรวจสอบให้แน่ใจว่าจุดสิ้นสุดที่กําหนดเปิดใช้งาน และไม่ถูกบล็อกเนื่องจากไฟร์วอลล์</span><span class="sxs-lookup"><span data-stu-id="e9682-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="e9682-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="e9682-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="e9682-108">การลงทะเบียนอาจล้มเหลวเนื่องจากการสื่อสารขาออกต้องผ่านการตรวจสอบ SSL โดยชั้นเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="e9682-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="e9682-109">ตรวจสอบให้แน่ใจว่าคุณได้ตรวจสอบการตั้งค่าการแจ้งเตือนของ Azure AD Connect Health แล้ว</span><span class="sxs-lookup"><span data-stu-id="e9682-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="e9682-110">โปรดตรวจสอบการตั้งค่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="e9682-110">Please review your setting.</span></span> <span data-ttu-id="e9682-111">คู่มือ [นี้](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) สามารถช่วยให้คุณเข้าใจวิธีการกําหนดค่าการตั้งค่าการแจ้งเตือนการแจ้งเตือนสถานภาพ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e9682-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="e9682-112">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับรายงานการซิงค์ AAD Connect Health และวิธีดาวน์โหลด ให้ดู [รายงานการซิงโครไนซ์ระดับ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)วัตถุ</span><span class="sxs-lookup"><span data-stu-id="e9682-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="e9682-113">เมื่อต้องการแก้ไขปัญหาการแจ้งเตือน AAD Connect Health ให้ปฏิบัติตามคู่มือการแก้ไขปัญหาของการแจ้งเตือนความสมบูรณ์ของข้อมูล [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) และถามบ่อย ให้ดูข้อถามการติดตั้ง [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)ทั่วไป</span><span class="sxs-lookup"><span data-stu-id="e9682-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
