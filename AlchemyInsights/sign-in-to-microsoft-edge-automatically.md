---
title: ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398748"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="5d63f-102">ลงชื่อเข้าใช้ Microsoft Edge โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5d63f-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="5d63f-103">Microsoft Edge ใช้บัญชีเริ่มต้นของ OS เพื่อลงชื่อเข้าใช้ผู้ใช้โดยอัตโนมัติตามวิธีกําหนดค่าอุปกรณ์ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="5d63f-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="5d63f-104">สถานการณ์สมมติของการกําหนดค่าอุปกรณ์แต่ละชนิดและขั้นตอนการลงชื่อเข้าใช้ของผู้ใช้ที่ไม่เป็นอิสระมีอธิบายไว้ด้านล่าง:</span><span class="sxs-lookup"><span data-stu-id="5d63f-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="5d63f-105">**อุปกรณ์นี้เป็นแบบไฮบริด/AAD-J:** ตัวเลือกนี้จะพร้อมใช้งานบน Windows 10, Windows ระดับลง และเวอร์ชันเซิร์ฟเวอร์ที่สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="5d63f-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="5d63f-106">ผู้ใช้จะลงชื่อเข้าใช้ด้วยบัญชี Azure Active Directory (AD) ของพวกเขาโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5d63f-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="5d63f-107">**อุปกรณ์ถูกรวมโดเมน**: ตัวเลือกนี้จะพร้อมใช้งานบน Windows 10, Windows ระดับลง และเวอร์ชันเซิร์ฟเวอร์ที่สอดคล้องกัน</span><span class="sxs-lookup"><span data-stu-id="5d63f-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="5d63f-108">ตามค่าเริ่มต้น ผู้ใช้ที่มีบัญชีผู้ใช้โดเมนจะไม่ลงชื่อเข้าใช้โดยอัตโนมัติ เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้อัตโนมัติให้กับพวกเขา ให้ใช้นโยบาย **ConfigureOnPremisesAccountAutoSignIn**</span><span class="sxs-lookup"><span data-stu-id="5d63f-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="5d63f-109">เมื่อต้องการเปิดใช้งานการลงชื่อเข้าใช้อัตโนมัติให้กับผู้ใช้ที่มีบัญชี Azure AD ให้พิจารณาการเข้าร่วมอุปกรณ์แบบไฮบริด</span><span class="sxs-lookup"><span data-stu-id="5d63f-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="5d63f-110">**บัญชีเริ่มต้นของระบบปฏิบัติการ** คือบัญชี Microsoft : ตัวเลือกนี้จะพร้อมใช้งานใน Windows 10 RS3 (เวอร์ชัน 1709 รุ่น 10.0.16299) และเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="5d63f-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="5d63f-111">สถานการณ์ไม่น่าเกิดขึ้นบนอุปกรณ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="5d63f-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="5d63f-112">แต่ถ้าบัญชีเริ่มต้นของ OS เป็นบัญชี Microsoft แล้ว Microsoft Edge จะลงชื่อเข้าใช้ผู้ใช้ด้วยบัญชี Microsoft โดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="5d63f-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
