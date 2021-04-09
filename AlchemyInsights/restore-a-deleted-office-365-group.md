---
title: คืนค่ากลุ่ม Microsoft 365 ที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645150"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="05066-102">คืนค่ากลุ่ม Microsoft 365 ที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="05066-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="05066-103">คุณสามารถคืนค่ากลุ่ม Microsoft 365 หรือ Microsoft Teams ที่ถูกลบภายใน 30 วันจากการลบ</span><span class="sxs-lookup"><span data-stu-id="05066-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="05066-104">ไปที่ศูนย์ [การจัดการ Microsoft 365](https://aka.ms/RestoreDeletedGroup) เพื่อเข้าสู่ระบบรายการของคุณคือกลุ่มและทีมที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="05066-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="05066-105">**หมายเหตุ:** เข้าสู่ระบบโดยใช้บัญชีที่มอบหมายให้ผู้ดูแลผู้เช่าหรือบทบาทผู้ดูแลกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="05066-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="05066-106">เลือกกลุ่ม Microsoft 365/Teams ที่ถูกลบเพื่อคืนค่า **และคลิกคืนค่า** กลุ่ม</span><span class="sxs-lookup"><span data-stu-id="05066-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="05066-107">ถ้ากลุ่มไม่สามารถคืนค่าได้เนื่องจากที่อยู่ SMTP ที่ขัดแย้งกัน ให้ใช้สั่งต่อไปนี้เพื่อค้นหาวัตถุที่ทําให้เกิดข้อขัดแย้งและเอาที่อยู่ SMTP ออก:</span><span class="sxs-lookup"><span data-stu-id="05066-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="05066-108">**หมายเหตุ:** ในบางกรณี อาจใช้เวลาถึง 24 ชั่วโมงในการคืนค่ากลุ่มและข้อมูลทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="05066-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="05066-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="05066-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>