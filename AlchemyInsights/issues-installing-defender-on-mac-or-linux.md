---
title: ปัญหาในการติดตั้ง Microsoft Defender บน Mac หรือ Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539699"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="1209f-102">ปัญหาในการติดตั้ง Microsoft Defender บน Mac หรือ Linux</span><span class="sxs-lookup"><span data-stu-id="1209f-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="1209f-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="1209f-103">**Mac**</span></span>

- <span data-ttu-id="1209f-104">ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะMicrosoft Defender ATP for Mac</span><span class="sxs-lookup"><span data-stu-id="1209f-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="1209f-105">ดูข้อมูลเพิ่มเติมได้ที่ วิธีการติดตั้ง[อุปกรณ์ Microsoft Defender ATP for](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)Mac</span><span class="sxs-lookup"><span data-stu-id="1209f-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="1209f-106">ตรวจทานข้อมูลในไฟล์: "/Library/Logs/Microsoft/mdatp/install.log"</span><span class="sxs-lookup"><span data-stu-id="1209f-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="1209f-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="1209f-107">**Linux**</span></span>

- <span data-ttu-id="1209f-108">ตรวจสอบให้แน่ใจว่าเป็นไปตามความต้องการของระบบก่อนที่จะติดตั้งMicrosoft Defender ATP For Linux</span><span class="sxs-lookup"><span data-stu-id="1209f-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="1209f-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="1209f-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="1209f-110">เมื่อต้องการตรวจสอบว่าบริการ MDATP ใช้งานอยู่ ให้ดู [การติดตั้ง](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)ล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="1209f-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="1209f-111">เมื่อต้องการแก้ไขปัญหาถ้าบริการไม่ได้เรียกใช้อยู่ ให้ดู [ขั้นตอนการแก้ไขปัญหาถ้าบริการ mdatp ไม่ได้](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)เรียกใช้อยู่</span><span class="sxs-lookup"><span data-stu-id="1209f-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="1209f-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="1209f-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="1209f-113">**หมายเหตุ** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="1209f-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>