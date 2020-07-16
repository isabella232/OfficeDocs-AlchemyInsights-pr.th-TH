---
title: เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148425"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="dd850-102">เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer</span><span class="sxs-lookup"><span data-stu-id="dd850-102">About identity in Yammer</span></span>

<span data-ttu-id="dd850-103">ขอแนะนําให้เครือข่ายทั้งหมดทําตามขั้นตอนต่อไปนี้เพื่อหลีกเลี่ยงปัญหาที่เกี่ยวข้องกับข้อมูลประจําตัว:</span><span class="sxs-lookup"><span data-stu-id="dd850-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="dd850-104">บังคับใช้ข้อมูลประจําตัวของ Office 365 หลังจากเตรียมใช้งานบัญชี Microsoft 365 สําหรับผู้ใช้ใน Azure AD เพื่อให้แน่ใจว่า ผู้ใช้ทุกคนเข้าสู่ระบบ โดยใช้บัญชี Microsoft 365 หลักของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="dd850-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="dd850-105">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การบังคับใช้ข้อมูลประจําตัวของ Office 365 สําหรับผู้ใช้ Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)</span><span class="sxs-lookup"><span data-stu-id="dd850-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="dd850-106">รวมเครือข่าย Yammer หลายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="dd850-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="dd850-107">การกําหนดค่า Yammer แบบดั้งเดิมอนุญาตให้หลายเครือข่าย Yammer สามารถเชื่อมต่อกับผู้เช่าหนึ่งราย</span><span class="sxs-lookup"><span data-stu-id="dd850-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="dd850-108">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การโยกย้ายเครือข่าย - รวมเครือข่าย Yammer หลายเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="dd850-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="dd850-109">หรือบังคับให้มีการอนุญาตให้ใช้สิทธิ์สําหรับ Yammer เพื่อบล็อกผู้ใช้จาก Yammer ถ้าผู้ใช้ไม่มีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="dd850-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="dd850-110">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="dd850-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="dd850-111">สุดท้าย ตรวจสอบรายการผู้ใช้สําหรับเครือข่าย Yammer รุ่นเก่า และระงับผู้ใช้แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="dd850-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="dd850-112">ขอแนะนําให้คุณระงับผู้ใช้ (ปิดใช้งาน) แทนการลบเนื่องจากการลบกลับไม่ได้</span><span class="sxs-lookup"><span data-stu-id="dd850-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="dd850-113">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ตรวจสอบผู้ใช้ Yammer ในเครือข่ายที่เชื่อมต่อกับ Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)และ[นําผู้ใช้ออก](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)</span><span class="sxs-lookup"><span data-stu-id="dd850-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="dd850-114">ด้วยการกําหนดค่า Yammer โดยใช้ขั้นตอนเหล่านี้ คุณจะพร้อมที่จะกําหนดค่าเครือข่าย Yammer ของคุณสําหรับโหมดดั้งเดิมสําหรับ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="dd850-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="dd850-115">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การตั้งค่าคอนฟิกเครือข่าย Yammer ของคุณสําหรับโหมดเนทิฟสําหรับ Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)</span><span class="sxs-lookup"><span data-stu-id="dd850-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>