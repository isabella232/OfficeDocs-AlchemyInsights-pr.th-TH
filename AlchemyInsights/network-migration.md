---
title: การย้ายเครือข่าย
ms.author: pebaum
author: pebaum
ms.date: 7/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 2fb66d68e131d22bc44f0fd878717d5e5e776dac
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734724"
---
# <a name="network-migration"></a><span data-ttu-id="20b2e-102">การย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="20b2e-102">Network Migration</span></span>

<span data-ttu-id="20b2e-103">ผู้เช่า O365 ของคุณอาจจะเกี่ยวข้องกับเครือข่าย Yammer หลายในผู้เช่า 1: การกำหนดค่าเครือข่ายจำนวนมาก</span><span class="sxs-lookup"><span data-stu-id="20b2e-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="20b2e-104">เริ่มต้น16ตุลาคม๒๐๑๘, Yammer จะไม่สนับสนุนเครือข่าย Yammer หลายที่เกี่ยวข้องกับผู้เช่า Office ๓๖๕หนึ่ง</span><span class="sxs-lookup"><span data-stu-id="20b2e-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one Office 365 tenant.</span></span> <span data-ttu-id="20b2e-105">คุณสามารถทำการโยกย้ายเครือข่ายเพื่อไปยังการกำหนดค่า1:1 ที่ต้องการได้</span><span class="sxs-lookup"><span data-stu-id="20b2e-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="20b2e-106">เมื่อต้องการดูรายการของเครือข่ายที่เชื่อมโยงกับผู้เช่าของคุณให้เข้าสู่ระบบ Yammer เป็นผู้ดูแลระบบส่วนกลางของ Office ๓๖๕และเรียกดูไปยัง**Admin เครือ**ข่ายจากนั้นการ**โยกย้ายเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="20b2e-106">To view a list of the networks associated with your tenant, log in to Yammer as an Office 365 Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="20b2e-107">เลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="20b2e-107">Choose **Next**.</span></span>

- <span data-ttu-id="20b2e-108">ถ้าคุณเห็นหลายเครือข่ายที่ระบุไว้ในขั้นตอนที่2จาก3คุณมีหลายเครือข่าย Yammer ที่เกี่ยวข้องกับผู้เช่า O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="20b2e-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="20b2e-109">หากต้องการแก้ไขการกำหนดค่าของคุณไปยังการกำหนดค่า1:1 ให้ดำเนินการต่อโดยใช้เครื่องมือการโยกย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="20b2e-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="20b2e-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการโยกย้ายเครือข่ายโปรดดูการ[โยกย้ายเครือข่าย: รวมหลายเครือข่าย Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="20b2e-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="20b2e-111">โปรดทราบ:</span><span class="sxs-lookup"><span data-stu-id="20b2e-111">Please Note:</span></span>
  
- <span data-ttu-id="20b2e-112">**การย้ายเครือข่ายจะย้ายเฉพาะผู้ใช้ที่ใช้งานอยู่และรอดำเนินการเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="20b2e-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="20b2e-113">ข้อมูลของผู้ใช้เช่นชื่อและรูปโปรไฟล์จะได้รับการโยกย้ายไปพร้อมกับผู้ใช้ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="20b2e-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="20b2e-114">เนื้อหาเครือข่ายใดๆรวมถึงกลุ่มจะไม่ถูกย้าย</span><span class="sxs-lookup"><span data-stu-id="20b2e-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="20b2e-115">**การโยกย้ายเครือข่ายไม่สามารถย้อนกลับได้**</span><span class="sxs-lookup"><span data-stu-id="20b2e-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="20b2e-116">คุณจะไม่สามารถเข้าถึงเครือข่ายของบริษัทสาขาและเนื้อหาหลังจากการย้ายข้อมูลได้</span><span class="sxs-lookup"><span data-stu-id="20b2e-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="20b2e-117">ดังนั้นก่อนที่คุณจะพิจารณาการโยกย้ายคุณต้องการวางแผนอย่างระมัดระวัง</span><span class="sxs-lookup"><span data-stu-id="20b2e-117">So before you consider a migration, you want to plan carefully.</span></span>
