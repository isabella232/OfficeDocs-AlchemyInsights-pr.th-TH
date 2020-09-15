---
title: ตรวจสอบบัญชีบริการ AADConnect
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1726"
- "9000180"
ms.openlocfilehash: 4c18ddc19c60075cbea4edce95ebbf6491778b41
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714050"
---
# <a name="check-the-aadconnect-service-accounts"></a><span data-ttu-id="32501-102">ตรวจสอบบัญชีบริการ AADConnect</span><span class="sxs-lookup"><span data-stu-id="32501-102">Check the AADConnect service accounts</span></span>

<span data-ttu-id="32501-103">ถ้าคุณได้รับข้อผิดพลาดการซิงโครไนซ์เช่น "ไม่มีการซิงโครไนซ์ล่าสุด" หรือสังเกตสถานะการซิงโครไนซ์ไดเรกทอรีในพอร์ทัลผู้ดูแลระบบ Office ระบุว่า "การซิงค์ล่าสุดมากกว่า3วันที่แล้ว" AADConnect อาจมีการตั้งค่าที่ไม่ถูกต้องหรือมีสิทธิ์ไม่เพียงพอที่จะทำการซิงโครไนซ์</span><span class="sxs-lookup"><span data-stu-id="32501-103">If you receive synchronization errors such as "No recent synchronization," or notice the directory synchronization status in the Office admin portal says "Last synced more than 3 days ago," AADConnect might have incorrect settings or insufficient permissions to perform a synchronization.</span></span> <span data-ttu-id="32501-104">การติดตั้งใหม่ AADConnect โดยใช้การตั้งค่าแบบด่วนอาจแก้ไขปัญหาได้</span><span class="sxs-lookup"><span data-stu-id="32501-104">Reinstalling AADConnect using express settings might resolve the issue.</span></span>

<span data-ttu-id="32501-105">เมื่อต้องการดาวน์โหลดเวอร์ชันล่าสุดของ AADConnect ให้ดูที่[เชื่อมต่อ Active directory ของ Microsoft Azure](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="32501-105">To download the latest version of AADConnect, see [Microsoft Azure Active Directory Connect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

<span data-ttu-id="32501-106">สำหรับคำแนะนำสำหรับการติดตั้งแบบด่วนให้ดู[ที่การเริ่มต้นใช้งาน AZURE AD Connect โดยใช้การตั้งค่าแบบด่วน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="32501-106">For instructions for express installation, see [Getting started with Azure AD Connect using express settings](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="32501-107">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับบัญชีผู้ใช้บริการ AADConnect ให้ดูที่[AZURE AD Connect: บัญชีผู้ใช้และสิทธิ์](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="32501-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>