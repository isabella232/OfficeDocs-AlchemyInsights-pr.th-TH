---
title: แก้ไขปัญหาการติดตั้ง MDATP บน Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696098"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="e4c05-102">แก้ไขปัญหาการติดตั้ง MDATP บน Mac</span><span class="sxs-lookup"><span data-stu-id="e4c05-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="e4c05-103">ถ้าการติดตั้งด้วยตนเองล้มเหลว **หน้าสรุป** ของตัวช่วยสร้างการติดตั้งจะแสดงข้อผิดพลาดต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e4c05-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="e4c05-104">"มีข้อผิดพลาดเกิดขึ้นในระหว่างการติดตั้ง</span><span class="sxs-lookup"><span data-stu-id="e4c05-104">"An error occurred during installation.</span></span> <span data-ttu-id="e4c05-105">ตัวติดตั้งพบข้อผิดพลาดที่เป็นสาเหตุให้การติดตั้งล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="e4c05-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="e4c05-106">ติดต่อผู้ผลิตซอฟต์แวร์เพื่อขอความช่วยเหลือ"</span><span class="sxs-lookup"><span data-stu-id="e4c05-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="e4c05-107">ในการปรับใช้ MDM หน้าจะแสดงการติดตั้งทั่วไปล้มเหลวเช่นกัน</span><span class="sxs-lookup"><span data-stu-id="e4c05-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="e4c05-108">แม้ว่าเราจะไม่แสดงข้อผิดพลาดที่แน่นอนต่อผู้ใช้ แต่เราเก็บไฟล์บันทึกที่มีความคืบหน้าการติดตั้งไว้ใน **/Library/Logs/Microsoft/mdatp/install.log**</span><span class="sxs-lookup"><span data-stu-id="e4c05-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="e4c05-109">เซสชันการติดตั้งแต่ละรายการจะผนวกเข้ากับไฟล์บันทึกนี้</span><span class="sxs-lookup"><span data-stu-id="e4c05-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="e4c05-110">เมื่อต้องการแสดงผลเซสชันการติดตั้งล่าสุด `sed` เท่านั้น ให้ใช้</span><span class="sxs-lookup"><span data-stu-id="e4c05-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="e4c05-111">หากต้องการเรียนรู้เพิ่มเติม โปรดดู[การแก้ไขปัญหาการติดตั้งของ Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="e4c05-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
