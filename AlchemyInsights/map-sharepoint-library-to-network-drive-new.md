---
title: แมปSharePointไปยังไดรฟ์เครือข่าย
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 6b7cb38362baa26bd39fe7478ef6dd1971b5b063
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52542840"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="67a91-102">แมปSharePointไปยังไดรฟ์เครือข่าย</span><span class="sxs-lookup"><span data-stu-id="67a91-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="67a91-103">แทนที่จะแมปไดรฟ์เครือข่าย SharePointไฟล์ด้วยไคลเอ็นต์OneDriveการซิงค์ใหม่ ซึ่งมีการเข้าถึงไฟล์ได้ตามต้องการ</span><span class="sxs-lookup"><span data-stu-id="67a91-103">Instead of mapping a network drive, sync SharePoint files with the new OneDrive sync client, which provides Files On-Demand.</span></span> <span data-ttu-id="67a91-104">เข้าถึงไฟล์ของคุณทั้งหมดใน OneDriveโดยไม่ต้องใช้พื้นที่เก็บข้อมูลภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="67a91-104">Access all your files in OneDrive without using local storage space.</span></span> <span data-ttu-id="67a91-105">For more information, see [Sync SharePoint Teams files with your computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) and Save disk space with OneDrive Files [On-Demand for Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="67a91-105">For more information, see [Sync SharePoint and Teams files with your computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) and [Save disk space with OneDrive Files On-Demand for Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span>

<span data-ttu-id="67a91-106">ถ้าคุณเลือกแมปไดรฟ์แทนที่จะใช้ไคลเอ็นต์การซิงค์ OneDrive[ใหม่](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)ตรวจสอบให้แน่ใจว่าคุณได้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="67a91-106">If you choose to map a drive instead of using [the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88), make sure you follow these steps:</span></span>

- [<span data-ttu-id="67a91-107">แก้ไขปัญหาเครือข่ายที่แมปไดรฟ์ที่เชื่อมต่อกับ SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="67a91-107">Troubleshoot mapped network drives that connect to SharePoint Online</span></span>](/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [<span data-ttu-id="67a91-108">ข้อผิดพลาดการรับรองความถูกต้องจะเกิดขึ้นเมื่อไคลเอ็นต์ไม่มีการสนับสนุน TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="67a91-108">Authentication errors occur when client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

<span data-ttu-id="67a91-109">**หมายเหตุ:** ถ้าคุณใช้ Internet Explorer 10กับ Windows 8 หรือ Windows 7 และได้รับ **การเข้าถึง** ถูกปฏิเสธหรือเส้นทางไม่สามารถเข้าถึงได้เมื่อแมปไดรฟ์ ให้แก้ไขปัญหานี้โดยการติดตั้งการแก้ไข [ด่วนนี้](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)</span><span class="sxs-lookup"><span data-stu-id="67a91-109">**NOTE:** If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, resolve this problem by installing this [hotfix](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d).</span></span>