---
title: เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664189"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="78f39-102">เกี่ยวกับข้อมูลเฉพาะตัวใน Yammer</span><span class="sxs-lookup"><span data-stu-id="78f39-102">About identity in Yammer</span></span>

<span data-ttu-id="78f39-103">ขอแนะนำว่าเครือข่ายทั้งหมดจะทำตามขั้นตอนต่อไปนี้เพื่อหลีกเลี่ยงปัญหาที่เกี่ยวข้องกับข้อมูลเฉพาะตัว:</span><span class="sxs-lookup"><span data-stu-id="78f39-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="78f39-104">บังคับใช้ข้อมูลประจำตัวของ Office ๓๖๕หลังจากการเตรียมใช้งานบัญชีผู้ใช้ Microsoft ๓๖๕สำหรับผู้ใช้ใน Azure AD เพื่อให้แน่ใจว่าผู้ใช้ทั้งหมดลงชื่อเข้าใช้โดยใช้บัญชีผู้ใช้ Microsoft ๓๖๕หลักของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="78f39-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="78f39-105">สำหรับข้อมูลเพิ่มเติมให้ดูที่[บังคับใช้ข้อมูลประจำตัวของ Office ๓๖๕สำหรับผู้ใช้ Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)</span><span class="sxs-lookup"><span data-stu-id="78f39-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="78f39-106">รวมเครือข่าย Yammer หลายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="78f39-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="78f39-107">การกำหนดค่า Yammer ดั้งเดิมอนุญาตให้เครือข่าย Yammer หลายเครือข่ายเชื่อมต่อกับผู้เช่าหนึ่งราย</span><span class="sxs-lookup"><span data-stu-id="78f39-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="78f39-108">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[โยกย้ายเครือข่ายรวมเครือข่าย Yammer หลายเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="78f39-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="78f39-109">อีกวิธีหนึ่งคือบังคับให้มีสิทธิ์การใช้งานสำหรับ Yammer เพื่อบล็อกผู้ใช้จาก Yammer ถ้าพวกเขาไม่มีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="78f39-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="78f39-110">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่จัดการสิทธิ์การใช้งานของผู้ใช้ Yammer ใน Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="78f39-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="78f39-111">สุดท้ายให้ตรวจสอบรายชื่อผู้ใช้สำหรับเครือข่าย Yammer รุ่นเก่าและหยุดผู้ใช้แบบดั้งเดิม</span><span class="sxs-lookup"><span data-stu-id="78f39-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="78f39-112">ขอแนะนำให้คุณระงับ (ปิดใช้งาน) ผู้ใช้แทนที่จะลบออกเนื่องจากการลบจะไม่สามารถย้อนกลับได้</span><span class="sxs-lookup"><span data-stu-id="78f39-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="78f39-113">สำหรับข้อมูลเพิ่มเติมให้ดูการ[ตรวจสอบผู้ใช้ Yammer ในเครือข่ายที่เชื่อมต่อกับ Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)และ[เอาผู้ใช้ออก](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)</span><span class="sxs-lookup"><span data-stu-id="78f39-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="78f39-114">ด้วยการกำหนดค่า Yammer โดยใช้ขั้นตอนเหล่านี้คุณจะพร้อมที่จะกำหนดค่าเครือข่าย Yammer ของคุณสำหรับโหมด Native ของ Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="78f39-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="78f39-115">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่การกำหนดค่าเครือข่าย Yammer ของคุณสำหรับโหมด Native สำหรับ Microsoft ๓๖๕](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)</span><span class="sxs-lookup"><span data-stu-id="78f39-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>