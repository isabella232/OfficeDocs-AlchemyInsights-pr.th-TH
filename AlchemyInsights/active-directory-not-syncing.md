---
title: ไดเรกทอรีที่ใช้งานไม่ซิงค์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265275"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="3d217-102">ไดเรกทอรีที่ใช้งานไม่ซิงค์</span><span class="sxs-lookup"><span data-stu-id="3d217-102">Active Directory not syncing</span></span>

<span data-ttu-id="3d217-103">ถ้าคุณได้รับข้อผิดพลาดในการทำข้อมูลให้ตรงกันเช่น "ไม่มีการซิงโครไนส์ล่าสุด" หรือสังเกตสถานะการซิงโครไนส์ของไดเรกทอรีใน Office admin portal กล่าวว่า "การซิงค์ครั้งล่าสุดมากกว่า3วันที่ผ่านมา" อาจเป็นว่า AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือไม่ สิทธิ์ในการทำข้อมูลให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="3d217-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="3d217-104">การติดตั้งใหม่ AADConnect โดยใช้การตั้งค่าแบบด่วนอาจแก้ไขปัญหาได้อย่างรวดเร็ว:</span><span class="sxs-lookup"><span data-stu-id="3d217-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="3d217-105">[ดาวน์โหลดรุ่นล่าสุดของ AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="3d217-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="3d217-106">[ทำตามคำแนะนำสำหรับการติดตั้งแบบเร่งด่วน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="3d217-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="3d217-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับบัญชีบริการ AADConnect ให้ดูที่การ[เชื่อมต่อ AD Azure: บัญชีและสิทธิ์](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="3d217-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
