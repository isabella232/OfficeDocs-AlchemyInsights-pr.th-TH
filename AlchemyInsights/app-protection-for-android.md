---
title: การตั้งค่านโยบายการป้องกันแอป Android ใน Microsoft Intune
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003997"
- "7057"
ms.openlocfilehash: 327df6e0a901037cd929cb845f805466d9bd4eff
ms.sourcegitcommit: 81c86027933c06db08d264918f2698d9c9a1659a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/20/2020
ms.locfileid: "49447572"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a><span data-ttu-id="6aace-102">การตั้งค่านโยบายการป้องกันแอป Android ใน Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6aace-102">Android app protection policy settings in Microsoft Intune</span></span>

<span data-ttu-id="6aace-103">มีสามประเภทของการตั้งค่านโยบายการป้องกันแอปสำหรับอุปกรณ์ Android:</span><span class="sxs-lookup"><span data-stu-id="6aace-103">There are three categories of app protection policy settings for Android devices:</span></span>

<span data-ttu-id="6aace-104">**การป้องกันข้อมูล** ควบคุมวิธีการจัดการข้อมูลของบริษัทเช่นไม่ว่าข้อมูลจะสามารถคัดลอกหรือวางลงในแอปอื่นหรือไม่หรือจะสามารถถ่ายภาพหน้าจอของแอปได้</span><span class="sxs-lookup"><span data-stu-id="6aace-104">**Data protection** controls how company data is handled, such as, whether data can be copied or pasted to a different app or whether a screenshot can be taken of the app.</span></span> <span data-ttu-id="6aace-105">การตั้งค่ายังบังคับใช้การเข้ารหัสลับข้อมูลของบริษัทและจัดการว่าข้อมูลบางอย่างสามารถซิงค์กับแอปอุปกรณ์ท้องถิ่นเช่นรายชื่อผู้ติดต่อหรือเว็บเบราว์เซอร์ได้ด้วย</span><span class="sxs-lookup"><span data-stu-id="6aace-105">The settings also enforce encryption on company data and manage whether certain data can be synced with the native device apps, like the contact list or web browser.</span></span> <span data-ttu-id="6aace-106">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[การป้องกันข้อมูล](https://go.microsoft.com/fwlink/?linkid=2135259)</span><span class="sxs-lookup"><span data-stu-id="6aace-106">To learn more, see [Data protection](https://go.microsoft.com/fwlink/?linkid=2135259).</span></span>

<span data-ttu-id="6aace-107">เส้นบอกแนวความต้องการในการ **เข้าถึง** วิธีที่ผู้ใช้สามารถเข้าถึงแอป</span><span class="sxs-lookup"><span data-stu-id="6aace-107">**Access requirements** guides how users can access an app.</span></span> <span data-ttu-id="6aace-108">ตัวอย่างเช่นแอปไม่จำเป็นต้องให้ผู้ใช้ใส่ PIN หรือลายนิ้วมือเพื่อเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="6aace-108">For example, an app could require the user to enter a PIN or fingerprint to access it.</span></span> <span data-ttu-id="6aace-109">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่ความต้องการในการ[เข้าถึง](https://go.microsoft.com/fwlink/?linkid=2135260)</span><span class="sxs-lookup"><span data-stu-id="6aace-109">To learn more, see [Access requirements](https://go.microsoft.com/fwlink/?linkid=2135260).</span></span>

<span data-ttu-id="6aace-110">การเปิดใช้ตาม **เงื่อนไข** จะควบคุมการตั้งค่าความปลอดภัยการลงชื่อเข้าใช้สำหรับแอปเช่นค่า PIN สูงสุดที่พยายามใช้ก่อนที่จะปิดใช้งานหรือระบบปฏิบัติการขั้นต่ำที่จำเป็นสำหรับการเรียกใช้แอป</span><span class="sxs-lookup"><span data-stu-id="6aace-110">**Conditional launch** governs the sign-in security settings for an app, such as, the maximum PIN attempts before lockout or the minimum operating system needed to run the app.</span></span> <span data-ttu-id="6aace-111">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่การเปิดใช้งานตาม[เงื่อนไข](https://go.microsoft.com/fwlink/?linkid=2135507)</span><span class="sxs-lookup"><span data-stu-id="6aace-111">To learn more, see [Conditional launch](https://go.microsoft.com/fwlink/?linkid=2135507).</span></span>
