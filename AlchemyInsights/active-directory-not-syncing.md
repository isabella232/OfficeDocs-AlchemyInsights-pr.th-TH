---
title: ไดเรกทอรีที่ใช้งานอยู่ไม่ซิงค์
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697648"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="50b6e-102">ไดเรกทอรีที่ใช้งานอยู่ไม่ซิงค์</span><span class="sxs-lookup"><span data-stu-id="50b6e-102">Active Directory not syncing</span></span>

<span data-ttu-id="50b6e-103">ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลการดูแลระบบ Office ระบุว่า "การซิงค์ครั้งล่าสุดมากกว่า3วันที่แล้ว" อาจเป็นเพราะว่า AADConnect มีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ไม่เพียงพอที่จะทำการซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="50b6e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="50b6e-104">การติดตั้งใหม่ AADConnect โดยใช้การตั้งค่าแบบด่วนอาจแก้ไขปัญหาได้อย่างรวดเร็ว:</span><span class="sxs-lookup"><span data-stu-id="50b6e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="50b6e-105">[ดาวน์โหลดเวอร์ชันล่าสุดของ AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="50b6e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="50b6e-106">[ทำตามคำแนะนำสำหรับการติดตั้งแบบด่วน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="50b6e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="50b6e-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับบัญชีผู้ใช้บริการ AADConnect ให้ดูที่[AZURE AD Connect: บัญชีผู้ใช้และสิทธิ์](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="50b6e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
