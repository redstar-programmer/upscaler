# redstar upscaler
เครื่องมือการปรับขนาดวิดีโอที่ทรงพลัง ffmpeg, real-esrgan, flowframes-now รองรับ ** ui หลายภาษา **!

## 🌐การตั้งค่าภาษา / ภาษา
[한국어](https://github.com/redstar-programmer/upscaler/blob/main/README.md) | [English](https://github.com/redstar-programmer/upscaler/blob/main/README/README.en.md) | [日本語](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ja.md) | [中文](https://github.com/redstar-programmer/upscaler/blob/main/README/README.zh.md) |
[Français](https://github.com/redstar-programmer/upscaler/blob/main/README/README.fr.md) | [Deutsch](https://github.com/redstar-programmer/upscaler/blob/main/README/README.de.md) | [Español](https://github.com/redstar-programmer/upscaler/blob/main/README/README.es.md) | [Português](https://github.com/redstar-programmer/upscaler/blob/main/README/README.pt.md) |
[Русский](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ru.md) | [Italiano](https://github.com/redstar-programmer/upscaler/blob/main/README/README.it.md) | [Tiếng Việt](https://github.com/redstar-programmer/upscaler/blob/main/README/README.vi.md) | [Bahasa Indonesia](https://github.com/redstar-programmer/upscaler/blob/main/README/README.id.md) |
[ภาษาไทย](https://github.com/redstar-programmer/upscaler/blob/main/README/README.th.md) | [العربية](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align = "center">
  <strong> ffmpeg, Realesrgan, เครื่องมือปรับอัตราการปรับขนาดวิดีโอที่ใช้ Flowframes </strong> <br>
  <em> ฐาน GUI ล่าสุดการตั้งค่าที่ตั้งไว้ล่วงหน้าการสนับสนุนการประมวลผลไฟล์หลายรายการ </em>
</p>

-

ดาวน์โหลด: [release]

## ✨สปอนเซอร์ upscaler ของ redstar

คุณต้องการชอบโครงการนี้หรือสนับสนุนการพัฒนาหรือไม่?  
ช่วยคุณลักษณะที่ดีกว่าและการอัปเดตที่มั่นคงด้วยการสนับสนุนขนาดเล็ก!  

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)

> 💡ราคาเซิร์ฟเวอร์เวลาในการพัฒนาและกาแฟหนึ่งถ้วยเป็นพลังที่ยอดเยี่ยม ขอบคุณ!

## สารบัญ

- [👋บทนำ] (#introduction)  
-[💾การติดตั้งและการเตรียมการ] (#การติดตั้งและเตรียมการ)  
- [🔧ฟังก์ชั่นหลัก] (#main-function)  
-[🚀วิธีการใช้ (เริ่มต้นอย่างรวดเร็ว)] (#use-quick-start)  
-[⚙รายละเอียดคำอธิบาย] (#รายละเอียดฟังก์ชั่นการอธิบาย)  
- [🙏ขอบคุณ] (#ขอบคุณเขียน)  
- [📜ประวัติ] (#history)

## 👋บทนำ
** redstar upscaler ** เป็นเครื่องมือ GUI ที่ใช้ Python ที่เพิ่มระดับวิดีโอให้กับความละเอียดสูงโดยอัตโนมัติโดยใช้ `ffmpeg`, 'Real-Esrgan' และ 'Flowframes'

-การสกัดเฟรมวิดีโอ→การเพิ่มขึ้น→การรวมกันของวิดีโอในครั้งเดียว
-สนับสนุนสำหรับรุ่น Realesrgan ต่างๆ
-ตัวเลือกผ่าน flowframes
-การสกัดและประมวลผลอัตโนมัติ Codec Automatic
-ทำงานบนตำแหน่งเดิมหรือเส้นทางที่กำหนด

> ⚠พัฒนาและทดสอบในสภาพแวดล้อม Windows

ด้านล่างเชื่อมต่อกับ YouTube โดยคลิกที่หน้าจอการใช้งานอย่างง่าย <br>
[![Watch the demo](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "Watch on YouTube")

## 💾การติดตั้งและการเตรียมการ

1. การติดตั้งเครื่องมือภายนอกและการยืนยันตำแหน่งต่อไปนี้ (อย่างไรก็ตามไฟล์การแจกแจงประกอบด้วยไฟล์การติดตั้ง FFMPEG, REAL-ESRGAN และ FLOWFRAMES (ดูโปรแกรมในเส้นทาง)))
   - [ffmpeg] (https://www.ffmpe.org/download.html)
   -[real-esrgan] (https://github.com/xinntao/real-esrgan
   - [flowframes] (https://github.com/n00mkrad/flowframes) *(เลือก) *
2. เรียกใช้ upscaler.exe ของ Readstar หลังจาก UNZIP
3. ในกรณีของ FlowFrames รุ่นที่โหลดตามสภาพแวดล้อมของผู้ใช้อาจแตกต่างกันดังนั้นอย่าลืมเรียกใช้ FlowFrames จากนั้น <br> การแก้ไข AI AI และ RedStar Upscaler ของรุ่น Redstar upscaler ของโมเดล/flowframes_models.ini ต้องตรงกัน <br> โมเดลที่ยังไม่ได้โหลดจะแสดงความคิดเห็นผ่านหน้าจอ # และตรวจสอบให้แน่ใจว่าได้ตรวจสอบว่าลำดับโมเดลของหน้าต่างการตั้งค่าของ redstar upscaler นั้นถูกจับคู่กับลำดับโมเดลของ <br> flowframes หรือไม่

## 🔧ฟังก์ชั่นหลัก

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
-VIDEO การเลือกหลายอย่างและงานต่อเนื่อง
-ADD วิดีโอลาก/ดร็อป
-✅ว่าจะเรียกใช้โปรแกรมหลักและเลือกการเลือกโดยตรง
-โหมดการบันทึก Disk
-การสนับสนุนทางภาษา (15 ภาษา)
<br> <br>
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
-แอปพลิเคชั่นที่ตั้งไว้ล่วงหน้าและแอปพลิเคชันอัตโนมัติ
-การตรวจจับตัวแปลงสัญญาณเสียงและการตั้งค่าการตั้งค่า
-การตรวจจับแบบอัตโนมัติและการเลือกรุ่น Realesrgan
-FFMPEG รายละเอียด FlowFrames Real-esrgan
-การตั้งค่าตัวเลือกการเปลี่ยนแปลงตามเวอร์ชัน flowframes <br>
<br> <br>
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
-การยืนยันคำสั่งการดำเนินการตามลำดับ (สามารถคัดลอกและดำเนินการแยกต่างหากจาก CMD)
<br> <br>
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
-ความก้าวหน้าโดยรวมของงานหรู
-UPSCALE การยืนยันการบันทึก (ไฟล์บันทึกถูกสร้างเป็นวันที่ในโฟลเดอร์บันทึกในโฟลเดอร์จริง)
-การจัดเรียงผลลัพธ์ของผลลัพธ์หลังจากเสร็จสิ้นการทำงาน ([redstar] คำนำหน้า)
-การดำเนินการในการดำเนินการหลังจากเสร็จสิ้น <br>
<br> <br>
## 🚀วิธีใช้ (เริ่มต้นอย่างรวดเร็ว)

1. เพิ่มไฟล์วิดีโอ (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WebM, 3GP, OGV)
2. ตรวจสอบตำแหน่งการทำงานหรือ "ใช้เส้นทางไฟล์ต้นฉบับ"
3. คลิกปุ่ม "การตั้งค่า" ในวิดีโอที่เพิ่มเข้ามา
4. ffmpeg, Realesrgan, รายละเอียด flowframes
5. คลิกใช้เฉพาะไฟล์ทั้งหมด / เลือกไฟล์
4. คลิกที่ปุ่มยืนยันงาน
7. คลิกที่ปุ่มเริ่มหลังจากตรวจสอบคำสั่งเพื่อเรียกใช้

> ✨ผลการทำงานถูกสร้างขึ้นในโฟลเดอร์ที่เลือกโดยสองภาพที่มีการปรับขนาดสองภาพและไฟล์วิดีโอที่ถูกแทรกสองเฟรม
> ✨ไฟล์ที่เสร็จสมบูรณ์จะถูกบันทึกเป็นชื่อไฟล์ที่มีคำนำหน้า [redstar]
-

## ⚙รายละเอียดคำอธิบาย

- รายการ | คำอธิบาย |
- - -
- ** การตั้งค่าเส้นทางงาน ** | ระบุเส้นทางเริ่มต้นหรือ "ใช้พา ธ ไฟล์ต้นฉบับ" |
- ** การสนับสนุนรูปแบบวิดีโอ ** | MP4, MKV, AVI, MOV, FLV, WMV, MPG, WebM, 3GP, OGV ฯลฯ
- ** รุ่นหรู ** | Realesr-animevideov3, Realesr-General, 4xPlus ฯลฯ
- ** การประมวลผลเสียง ** | การสนับสนุนการเข้ารหัสรูปแบบต่างๆเช่น 'AAC', 'MP3' และ 'FLAC' |
- ** flowframes เชื่อมโยง ** | ตั้งค่าการแก้ไข (FPS × 2, × 4, × 8) |
- ** โหมดการออมดิสก์ ** | ฟังก์ชั่นการลบภาพอัตโนมัติระดับกลางให้

## 🙏วันขอบคุณพระเจ้า

- realesrgan by [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes by [n00mkrad](https://github.com/n00mkrad/flowframes)
-หากคุณต้องการมีส่วนร่วมในโครงการนี้หรือแนะนำฟังก์ชั่นโปรดแสดงความคิดเห็นเกี่ยวกับ [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).


# 📜ประวัติ

v 1.1.0
 - การกำหนดค่าเมนู (เปิดไฟล์ปิดการตั้งค่าการตั้งค่าภาษา)
 > 2. เพิ่มการตั้งค่าภาษาหลายภาษา (ภาษาที่มีอยู่: เกาหลี, อังกฤษ, 日本語, 中文, Français, Deutsch, Español, Português, рский, TiếngViệt, Bahasa Indonesia ال)
 3. ข้อความและการเปลี่ยนแปลงรหัสบางอย่างตามการเพิ่มการตั้งค่าภาษา
 > 4. การเปลี่ยนแปลงการกำหนดค่า UI บางอย่าง
 - ffmpeg, real-esrgan, flowframes ข้อมูลแต่ละรุ่น (หน้าจอหลัก)
 > 6. การตอบสนอง FlowFrames 1.41.0 (เวอร์ชันปัจจุบัน 1.41.0 มีปัญหาคำสั่ง CMD ดังนั้นสามารถใช้เพียง 1.40.0 และ 1.36.0)
 > แก้ปัญหาที่รายการโมเดล AI จะแสดงเป็นตัวพิมพ์เล็ก
 8. ตัวเลือก FFMPEG (พิกเซล, วิดีโอตัวแปลงสัญญาณ)
 > 9. การเสริมแรงของ CUDA ตรวจสอบพีซีผู้ใช้ -สามารถใช้และตรวจสอบประเภทของ GPU (หน้าจอหลัก)

v 1.0.0
 -
 - การเปลี่ยนแปลง UI
 > 3. ช่วงวิดีโอ/เสียงที่เพิ่มขึ้นได้เพิ่มขึ้น
 > 4. เพิ่มโหมดการบันทึกดิสก์
 > การกระจายรวมถึงโปรแกรมหลัก ๆ

v 0.1.92
 - flowframes ปัญหาของความล้มเหลวในการแก้ไขโดยการป้อนข้อมูลซ้ำในกล่องคอมโบโมเดล AI เมื่อเปลี่ยนเส้นทาง
 > 2. เพิ่มสถานะการเลือกของกล่องคอมโบสำหรับงานแก้ไข

v 0.1.91
 -
 > 2. การปรับไฟล์แจกจ่าย

v 0.1.9
 - แอปพลิเคชันเปลี่ยนโมเดล flowframes
 - FlowFrames 1.36.0 รุ่นใหม่, การใช้งานรุ่น 1.40.0
 3. ไม่มีคำสั่ง flowframes เกิดขึ้นอีกต่อไปอีกต่อไป
 > 4. คุณสามารถเพิ่มไฟล์ด้วยการลาก/ดร็อป
 > แก้ปัญหาที่ไม่ได้ใช้

v 0.1.8
 -
 2. หากติดตั้ง flowframes ในพา ธ เริ่มต้น (เช่น C: \ users \ Administrator
 3. เมื่อเพิ่มหลายไฟล์ 
 > 4. หลังจากเพิ่มหลายไฟล์

v 0.1.7
 - การเปลี่ยนขนาดโปรแกรม
 2. แก้ปัญหาข้อผิดพลาดเมื่อทำงานกับไฟล์โดยไม่มีเสียง
 > 3. เปลี่ยนการกำหนดค่า UI ทั้งหมด (กำหนดค่าใหม่เพื่อให้พอดีกับการเปลี่ยนขนาด)

v 0.1.6
 -
 - แก้ปัญหาที่ข้อมูลเวอร์ชันไม่ได้ถูกมองว่าเป็นเวอร์ชันใหม่ในชื่อโปรแกรม
 > แก้ปัญหาที่เก็บไฟล์ config.ini ไว้ในเส้นทางอื่น ๆ
 > 4. เมื่อเปลี่ยนการระบายน้ำระดับสูง Realesrgan กล่องคอมโบรุ่นหรูจะเปลี่ยนไปด้วยกัน
 > 5. เพิ่มฟังก์ชั่นตรวจสอบอัปเดต
 > 6. การปรับเปลี่ยนตรรกะบางอย่าง
 > 7. ความละเอียดและ FPS
 > 8. การแก้ไขความละเอียด (อดีต) ผู้ใช้ (ต้องป้อนในรูปแบบของ 1024x768)

v 0.1.5
 -
 2.
 3. เพิ่มวิดีโอบางส่วนของกล่องคอมโบ "การคำนวณ FPS" เพื่อป้องกันไม่ให้เคสถูกคำนวณเป็น FPS ที่ไม่ถูกต้องเมื่อคำนวณ FPS ของวิดีโอบางรายการ
        -> สามารถเลือก r_frame_rate / avg_frame_rate ได้และค่าเริ่มต้นจะคำนวณโดย r_frame_rate
 > 4. เมื่อเลือกไฟล์วิดีโอความคืบหน้าของข้อมูลวิดีโอ 
 > 5. หลังจากเตะไฟล์แล้วให้เปลี่ยนเพื่อเปิดโฟลเดอร์ที่เลือกล่าสุดโดยค่าเริ่มต้นเมื่อเลือกไฟล์อีกครั้ง

v 0.1.4
 - config.ini วิธีการอ่านไฟล์เปลี่ยน
 > 2. เปลี่ยนข้อมูลวิดีโอจาก Python av เป็น ffmpeg
 > 3. เพิ่มฟังก์ชั่น Windows End เมื่อทำงานในการทำงาน
 > 4. ในรายการงานชื่อไฟล์ทั้งหมดจะแสดงเป็นคำแนะนำเครื่องมือ
 - ในรายการงานความละเอียดของไฟล์แต่ละไฟล์ (ก่อน) / ความละเอียด (หลังจาก) / fps (ก่อน) / fps (โพสต์) สัญกรณ์
 > 6. การถอดกล่องอินพุต FPS (การลบเนื่องจากแต่ละไฟล์)
 > 7. เอาท์พุท FPS ขนาดการพยากรณ์ขนาดการกำจัด (การลบเนื่องจากแต่ละไฟล์สำหรับแต่ละไฟล์)
 > 8. สถานะความคืบหน้าถูกเขียนเป็นสอง proessbar โดยไฟล์/งานเต็มรูปแบบ

v 0.1.3
 > 1. แก้ไขข้อผิดพลาดการคำนวณไฟล์ FPS ด้วยข้อมูล FPS บางส่วนเมื่อนำเข้าไฟล์

v 0.1.2
 - การเปลี่ยนแปลงการกำหนดค่า UI   
 > 2. การเปลี่ยนแปลงตรรกะภายใน  
 > แก้ปัญหาที่ไม่ได้ดำเนินการเมื่อเลือกสองรุ่นด้านล่างระหว่างรุ่น Realesrgan  
 > 4. เปลี่ยนวิธีใช้โมเดล Realesrgan   
 > -> คัดลอกไฟล์รุ่นใหม่ (*.Param) ไปยังโฟลเดอร์โมเดลในโฟลเดอร์การติดตั้ง RealesRgan  
 -  
 > 6. config.ini รหัสการย้ายไฟล์  
 > 7. Ffmpeg Decomposition Image AAC-> FLAC  
 > 8. การดัดแปลงข้อผิดพลาดอื่น ๆ

v 0.1.1
 - การเขียนครั้งแรก, ffmepg, realesrgan และ flowframes