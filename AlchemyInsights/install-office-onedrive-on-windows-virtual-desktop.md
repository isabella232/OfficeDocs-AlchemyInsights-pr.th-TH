---
title: ติดตั้ง Office และ OneDrive บนเดสก์ท็อปเสมือนของ Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596031"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="48bef-102">ติดตั้ง Office และ OneDrive บนเดสก์ท็อปเสมือนของ Windows</span><span class="sxs-lookup"><span data-stu-id="48bef-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="48bef-103">[เตรียมและปรับแต่งภาพ VHD ต้นแบบ](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="48bef-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="48bef-104">สร้างเครื่องเสมือน (VM) ถ้ายังไม่ได้สร้าง</span><span class="sxs-lookup"><span data-stu-id="48bef-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="48bef-105">[ติดตั้ง Office ในโหมดการเปิดใช้งานคอมพิวเตอร์ที่](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)แชร์</span><span class="sxs-lookup"><span data-stu-id="48bef-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="48bef-106">การเปิดใช้งานคอมพิวเตอร์ที่แชร์อนุญาตให้ผู้ใช้หลายคนเข้าถึง Office ได้</span><span class="sxs-lookup"><span data-stu-id="48bef-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="48bef-107">[ติดตั้ง OneDrive ในโหมดต่อเครื่อง](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="48bef-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="48bef-108">โดยปกติแล้ว OneDrive จะถูกติดตั้งต่อผู้ใช้ แต่ที่นี่ควรติดตั้งต่อเครื่อง</span><span class="sxs-lookup"><span data-stu-id="48bef-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>