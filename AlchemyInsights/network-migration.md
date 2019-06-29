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
ms.openlocfilehash: 08f7c7f2a36a77e460ad1bc2ce78e40072133e6e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379156"
---
# <a name="network-migration"></a><span data-ttu-id="3b0f0-102">การย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="3b0f0-102">Network Migration</span></span>

<span data-ttu-id="3b0f0-103">ผู้เช่า O365 ของคุณคืออาจเกี่ยวข้องกับหลายเครือข่าย Yammer ในผู้เช่า 1: ตั้งค่าคอนฟิกเครือข่ายมากขึ้น</span><span class="sxs-lookup"><span data-stu-id="3b0f0-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="3b0f0-104">เริ่ม 16 ตุลาคม 2018, Yammer จะไม่สนับสนุนเครือข่าย Yammer หลายที่เกี่ยวข้องกับผู้เช่า Office 365 หนึ่ง</span><span class="sxs-lookup"><span data-stu-id="3b0f0-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one Office 365 tenant.</span></span> <span data-ttu-id="3b0f0-105">คุณสามารถทำการโยกย้ายเครือข่ายจะได้รับการตั้งค่าคอนฟิก 1:1 ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="3b0f0-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="3b0f0-106">เมื่อต้องการดูรายการเครือข่ายเชื่อมโยงกับผู้เช่าของคุณ ล็อกอินไปยัง Yammer เป็น Office 365 สากลผู้ดูแลระบบ และเรียกดู**ผู้ดูแลเครือข่าย**แล้ว**ย้ายเครือข่าย**</span><span class="sxs-lookup"><span data-stu-id="3b0f0-106">To view a list of the networks associated with your tenant, log in to Yammer as an Office 365 Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="3b0f0-107">เลือก**ถัดไป**</span><span class="sxs-lookup"><span data-stu-id="3b0f0-107">Choose **Next**.</span></span>

- <span data-ttu-id="3b0f0-108">ถ้าคุณเห็นหลายเครือข่ายที่มีอยู่ในขั้นตอนที่ 2 จาก 3 จาก นั้นคุณมีเครือข่าย Yammer หลายที่เกี่ยวข้องกับผู้เช่า O365 ของคุณ</span><span class="sxs-lookup"><span data-stu-id="3b0f0-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="3b0f0-109">เมื่อต้องการแก้ไขการตั้งค่าคอนฟิกของการตั้งค่าคอนฟิกเป็น 1:1 ดำเนินต่อโดยใช้เครื่องมือการย้ายเครือข่าย</span><span class="sxs-lookup"><span data-stu-id="3b0f0-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="3b0f0-110">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการย้ายเครือข่ายโปรดดู[เครือข่ายโยกย้าย: รวมหลายเครือข่าย Yammer](https://support.office.com/article/a22c1b20-9231-4ce2-a916-392b1056d002)</span><span class="sxs-lookup"><span data-stu-id="3b0f0-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://support.office.com/article/a22c1b20-9231-4ce2-a916-392b1056d002)</span></span>

<span data-ttu-id="3b0f0-111">โปรดทราบ:</span><span class="sxs-lookup"><span data-stu-id="3b0f0-111">Please Note:</span></span>
  
- <span data-ttu-id="3b0f0-112">**การโยกย้ายเครือข่ายย้ายเฉพาะการใช้งานและ รอให้ผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="3b0f0-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="3b0f0-113">พร้อม ด้วยผู้ใช้ที่ใช้งานอยู่ นอกจากนี้ยังมีโยกย้ายข้อมูลของผู้ใช้ เช่นรูปภาพชื่อและโปรไฟล์</span><span class="sxs-lookup"><span data-stu-id="3b0f0-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="3b0f0-114">ไม่มีโยกย้ายเนื้อหาใด ๆ บนเครือข่าย กลุ่ม รวม</span><span class="sxs-lookup"><span data-stu-id="3b0f0-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="3b0f0-115">**การย้ายเครือข่ายไม่สามารถย้อนกลับ**</span><span class="sxs-lookup"><span data-stu-id="3b0f0-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="3b0f0-116">คุณจะไม่สามารถเข้าถึงเครือข่ายของบริษัทในเครือและเนื้อหาหลังจากโยกย้าย</span><span class="sxs-lookup"><span data-stu-id="3b0f0-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="3b0f0-117">ดังนั้น ก่อนที่คุณควรพิจารณาการโยกย้าย คุณต้องวางแผนอย่างระมัดระวัง</span><span class="sxs-lookup"><span data-stu-id="3b0f0-117">So before you consider a migration, you want to plan carefully.</span></span>
