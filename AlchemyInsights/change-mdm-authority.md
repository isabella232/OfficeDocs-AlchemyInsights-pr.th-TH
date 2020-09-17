---
title: เปลี่ยนแปลงหน่วยงาน MDM
ms.author: sirkkuw
author: Sirkkuw
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 08c51aa6-cffc-456b-91fb-185f0d636afb
ms.openlocfilehash: f336ef2b84dcc7a44c6b603e2fbdb1aa08bd367d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793849"
---
# <a name="change-intune-mdm-authority"></a><span data-ttu-id="606f7-102">การเปลี่ยนแปลงสิทธิ์การ MDM ของ Intune</span><span class="sxs-lookup"><span data-stu-id="606f7-102">Change Intune MDM authority</span></span>

<span data-ttu-id="606f7-103">คุณสามารถเปลี่ยนสิทธิ์การใช้งาน MDM ของคุณได้โดยไม่ต้องเปิดกรณีสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="606f7-103">You can change your MDM authority without opening a support case.</span></span> <span data-ttu-id="606f7-104">ดูเอกสารต่อไปนี้สำหรับคำแนะนำ:</span><span class="sxs-lookup"><span data-stu-id="606f7-104">See the following documents for instructions:</span></span>
  
- [<span data-ttu-id="606f7-105">เปลี่ยนสิทธิ์ MDM ของคุณจากตัวจัดการการกำหนดค่าไปยัง Intune แบบสแตนด์อโลน</span><span class="sxs-lookup"><span data-stu-id="606f7-105">Change your MDM authority from Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/configmgr/mdm/deploy-use/migrate-change-mdm-authority)
    
- [<span data-ttu-id="606f7-106">เปลี่ยนสิทธิ์ MDM ของคุณจาก Intune แบบสแตนด์อโลนไปยังตัวจัดการการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="606f7-106">Change your MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/configmgr/mdm/deploy-use/change-mdm-authority)
    
 <span data-ttu-id="606f7-107">**การมีสิทธิ์ร่วมกันของ MDM**</span><span class="sxs-lookup"><span data-stu-id="606f7-107">**MDM Authority Co-Existence**</span></span>
  
- <span data-ttu-id="606f7-108">คุณสามารถมีทั้งเจ้าหน้าที่ MDM ที่ใช้งานอยู่พร้อมกันถ้าคุณมี Office ๓๖๕ MDM เปิดใช้งานแล้วแต่คุณต้องการลองใช้ Intune MDM</span><span class="sxs-lookup"><span data-stu-id="606f7-108">You can have both MDM authorities active concurrently if you already have Office 365 MDM enabled but you want to try Intune MDM.</span></span>
    
- <span data-ttu-id="606f7-109">ผู้ดูแลระบบที่มี O365 MDM ใช้งานอยู่แล้วก็สามารถทำเครื่องหมายได้ด้วยการใช้งานด้วยตัวเองของ Intune ที่ใช้งานอยู่จากพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="606f7-109">Admins who already have O365 MDM active can simply mark Intune MDM as active from the Azure portal.</span></span>
    
- <span data-ttu-id="606f7-110">ถ้าคุณมี Intune MDM แต่ต้องการใช้ Office ๓๖๕ MDM: โปรดเปิดบัตรที่ด้านล่างและตัวแทนฝ่ายสนับสนุนจะช่วยให้คุณสามารถทำสิ่งนี้ได้</span><span class="sxs-lookup"><span data-stu-id="606f7-110">If you have Intune MDM but want to make use of Office 365 MDM: please open a ticket below and a support agent will help enable this for you.</span></span>
    

