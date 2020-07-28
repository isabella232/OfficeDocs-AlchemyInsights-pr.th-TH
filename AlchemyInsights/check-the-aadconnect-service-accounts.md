---
title: ตรวจสอบบัญชีบริการ AADConnect
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1726"
- "9000180"
ms.openlocfilehash: 49498a50f9bb0c26bef1959c3d1eff6dd8f0e2bc
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439936"
---
# <a name="check-the-aadconnect-service-accounts"></a><span data-ttu-id="58e53-102">ตรวจสอบบัญชีบริการ AADConnect</span><span class="sxs-lookup"><span data-stu-id="58e53-102">Check the AADConnect service accounts</span></span>

<span data-ttu-id="58e53-103">ถ้าคุณได้รับข้อผิดพลาดในการซิงโครไนส์เช่น "ไม่มีการซิงโครไนส์ล่าสุด" หรือสังเกตเห็นสถานะการซิงโครไนส์ไดเรกทอรีในพอร์ทัลผู้ดูแลระบบ Office แจ้งว่า "ซิงค์ล่าสุดมากกว่า 3 วันที่ผ่านมา" AADConnect อาจมีการตั้งค่าที่ไม่ถูกต้องหรือสิทธิ์ไม่เพียงพอที่จะทําข้อมูลให้ตรงกัน</span><span class="sxs-lookup"><span data-stu-id="58e53-103">If you receive synchronization errors such as "No recent synchronization," or notice the directory synchronization status in the Office admin portal says "Last synced more than 3 days ago," AADConnect might have incorrect settings or insufficient permissions to perform a synchronization.</span></span> <span data-ttu-id="58e53-104">การติดตั้ง AADConnect ใหม่โดยใช้การตั้งค่าแบบด่วนอาจช่วยแก้ปัญหาได้</span><span class="sxs-lookup"><span data-stu-id="58e53-104">Reinstalling AADConnect using express settings might resolve the issue.</span></span>

<span data-ttu-id="58e53-105">เมื่อต้องการดาวน์โหลดรุ่นล่าสุดของ AADConnect ดู[Microsoft Azure ที่ใช้งานอยู่ไดเรกทอรีเชื่อมต่อ](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="58e53-105">To download the latest version of AADConnect, see [Microsoft Azure Active Directory Connect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

<span data-ttu-id="58e53-106">สําหรับคําแนะนําสําหรับการติดตั้งแบบด่วน ให้ดูที่[การเริ่มต้นใช้งาน Azure AD Connect โดยใช้การตั้งค่าแบบด่วน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="58e53-106">For instructions for express installation, see [Getting started with Azure AD Connect using express settings](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="58e53-107">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับบัญชีบริการ AADConnect ให้ดูที่[การเชื่อมต่อโฆษณา Azure: บัญชีและสิทธิ์](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="58e53-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>