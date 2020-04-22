---
title: การย้ายเครือข่าย
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: aada8e90d168a4c621dd81ee8d306b934c20d119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761833"
---
# <a name="network-migration"></a><span data-ttu-id="040d4-102">การย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="040d4-102">Network Migration</span></span>

<span data-ttu-id="040d4-103">ผู้เช่า O365 ของคุณอาจเกี่ยวข้องกับเครือข่าย Yammer หลายในผู้เช่า 1 : การกําหนดค่าเครือข่ายจํานวนมาก</span><span class="sxs-lookup"><span data-stu-id="040d4-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="040d4-104">เริ่มต้น 16 ตุลาคม 2018 Yammer จะไม่สนับสนุนเครือข่าย Yammer หลายเครือข่ายที่เชื่อมโยงกับผู้เช่าหนึ่ง</span><span class="sxs-lookup"><span data-stu-id="040d4-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="040d4-105">คุณสามารถดําเนินการย้ายข้อมูลเครือข่ายเพื่อไปยังการกําหนดค่าแบบ 1:1 ที่ต้องการได้</span><span class="sxs-lookup"><span data-stu-id="040d4-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="040d4-106">เมื่อต้องการดูรายการของเครือข่ายที่เกี่ยวข้องกับผู้เช่าของคุณ ให้ล็อกอินไปยัง Yammer ในฐานะผู้ดูแลระบบส่วนกลาง และเรียกดู**ผู้ดูแลระบบเครือข่าย**แล้ว**ย้ายเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="040d4-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="040d4-107">เลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="040d4-107">Choose **Next**.</span></span>

- <span data-ttu-id="040d4-108">ถ้าคุณเห็นหลายเครือข่ายที่แสดงรายการในขั้นตอนที่ 2 จาก 3 แล้วคุณมีเครือข่าย Yammer หลายที่เกี่ยวข้องกับผู้เช่า O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="040d4-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="040d4-109">เมื่อต้องการแก้ไขการกําหนดค่าของคุณไปยังการกําหนดค่าแบบ 1:1 ให้ใช้เครื่องมือการโยกย้ายเครือข่ายต่อไป</span><span class="sxs-lookup"><span data-stu-id="040d4-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="040d4-110">สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการย้ายเครือข่าย โปรดดูที่[การโยกย้ายเครือข่าย: รวมเครือข่าย Yammer หลายเครือข่าย](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="040d4-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="040d4-111">หมายเหตุ:</span><span class="sxs-lookup"><span data-stu-id="040d4-111">Please Note:</span></span>
  
- <span data-ttu-id="040d4-112">**การย้ายข้อมูลเครือข่ายจะย้ายเฉพาะผู้ใช้ที่ใช้งานอยู่และที่รอดําเนินการเท่านั้น**</span><span class="sxs-lookup"><span data-stu-id="040d4-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="040d4-113">ข้อมูลของผู้ใช้ เช่น ชื่อและรูปโปรไฟล์จะถูกย้ายด้วย</span><span class="sxs-lookup"><span data-stu-id="040d4-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="040d4-114">เนื้อหาเครือข่ายใดๆ รวมถึงกลุ่มจะไม่ถูกย้าย</span><span class="sxs-lookup"><span data-stu-id="040d4-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="040d4-115">**ไม่สามารถย้อนกลับการโยกย้ายเครือข่ายได้**</span><span class="sxs-lookup"><span data-stu-id="040d4-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="040d4-116">คุณจะไม่สามารถเข้าถึงเครือข่ายและเนื้อหาบริษัทในเครือของคุณได้หลังจากการย้ายข้อมูล</span><span class="sxs-lookup"><span data-stu-id="040d4-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="040d4-117">ดังนั้นก่อนที่คุณจะพิจารณาการย้ายที่คุณต้องการวางแผนอย่างรอบคอบ</span><span class="sxs-lookup"><span data-stu-id="040d4-117">So before you consider a migration, you want to plan carefully.</span></span>
