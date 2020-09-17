---
title: การโยกย้ายเครือข่าย
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799583"
---
# <a name="network-migration"></a><span data-ttu-id="a5b57-102">การโยกย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="a5b57-102">Network Migration</span></span>

<span data-ttu-id="a5b57-103">ผู้เช่า O365 ของคุณอาจเกี่ยวข้องกับเครือข่าย Yammer หลายเครือข่ายใน1ผู้เช่า: การกำหนดค่าเครือข่ายจำนวนมาก</span><span class="sxs-lookup"><span data-stu-id="a5b57-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="a5b57-104">เริ่มต้นวันที่16ตุลาคม๒๐๑๘ Yammer จะไม่สนับสนุนเครือข่าย Yammer หลายเครือข่ายที่เชื่อมโยงกับผู้เช่าหนึ่งรายอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="a5b57-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="a5b57-105">คุณสามารถดำเนินการโยกย้ายเครือข่ายเพื่อไปยังการกำหนดค่า1:1 ที่ต้องการได้</span><span class="sxs-lookup"><span data-stu-id="a5b57-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="a5b57-106">เมื่อต้องการดูรายการของเครือข่ายที่เชื่อมโยงกับผู้เช่าของคุณให้เข้าสู่ระบบ Yammer ในฐานะผู้ดูแลระบบส่วนกลางแล้วเรียกดู**ผู้ดูแลระบบเครือข่าย**จากนั้นการ**โยกย้ายเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="a5b57-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="a5b57-107">เลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="a5b57-107">Choose **Next**.</span></span>

- <span data-ttu-id="a5b57-108">ถ้าคุณเห็นหลายเครือข่ายที่แสดงรายการในขั้นตอนที่2จาก3คุณมีเครือข่าย Yammer หลายเครือข่ายที่เชื่อมโยงกับผู้เช่า O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="a5b57-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="a5b57-109">เมื่อต้องการแก้ไขการกำหนดค่าของคุณไปยังการกำหนดค่า1:1 ให้ดำเนินการต่อโดยใช้เครื่องมือการโยกย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="a5b57-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="a5b57-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการโยกย้ายเครือข่ายโปรดดูที่การ [โยกย้ายเครือข่าย: รวมเครือข่าย Yammer หลายเครือ](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)ข่าย</span><span class="sxs-lookup"><span data-stu-id="a5b57-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="a5b57-111">โปรดทราบว่า:</span><span class="sxs-lookup"><span data-stu-id="a5b57-111">Please Note:</span></span>
  
- <span data-ttu-id="a5b57-112">**การโยกย้ายเครือข่ายจะย้ายเฉพาะผู้ใช้ที่ใช้งานอยู่และที่ค้างอยู่**</span><span class="sxs-lookup"><span data-stu-id="a5b57-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="a5b57-113">พร้อมกับผู้ใช้ที่ใช้งานอยู่ข้อมูลของผู้ใช้เช่นชื่อและรูปโปรไฟล์จะถูกโยกย้ายไปด้วย</span><span class="sxs-lookup"><span data-stu-id="a5b57-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="a5b57-114">เนื้อหาเครือข่ายใดๆรวมถึงกลุ่มจะไม่ถูกโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="a5b57-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="a5b57-115">**การโยกย้ายเครือข่ายไม่สามารถย้อนกลับได้**</span><span class="sxs-lookup"><span data-stu-id="a5b57-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="a5b57-116">คุณจะไม่สามารถเข้าถึงเครือข่ายบริษัทในเครือของคุณและเนื้อหาหลังจากการโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="a5b57-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="a5b57-117">ดังนั้นก่อนที่คุณจะพิจารณาการโยกย้ายคุณต้องการวางแผนอย่างระมัดระวัง</span><span class="sxs-lookup"><span data-stu-id="a5b57-117">So before you consider a migration, you want to plan carefully.</span></span>
