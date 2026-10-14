# filling-holes-on-image-with-image-processing-with-Python

สรุป GitHub repo: opencv-filling-holes

Repo นี้เป็นตัวอย่างการเติมรู (fill holes) ในภาพไบนารีด้วย OpenCV + Python โดยอิงจากบทความของ LearnOpenCV

ไฟล์หลักใน repo

imfill.py — สคริปต์หลัก

nickel.jpg — ภาพตัวอย่างเหรียญนิกเกิล

example.jpg / example1.jpg — ภาพตัวอย่างเพิ่มเติม

README.md — คำอธิบายสั้น ๆ

หลักการทำงาน

OpenCV ไม่มีฟังก์ชัน imfill แบบ MATLAB โดยตรง จึงใช้วิธีนี้แทน:

อ่านภาพแล้วแปลงเป็น grayscale

Threshold แบบ THRESH_BINARY_INV (เช่น threshold = 220) เพื่อแยกขอบวัตถุออกจากพื้นหลัง

ใช้ FloodFill จากจุด (0,0) เพื่อเติมสีพื้นหลังด้านนอก

Invert ภาพที่ flood fill แล้ว

รวมภาพ threshold เดิมกับภาพที่ invert ด้วย bitwise OR → ได้ภาพที่รูภายในถูกเติมเต็ม

*****************************************************************************

Name : Patasu Daungmala

Position : R&D Manager

Tel : 0641900551

E-mail : nextsoftware.pp@gmail.com

Line : https://lin.ee/THH8PAt

Medium : https://dr-pathasu-doung.medium.com

Github : https://github.com/doungmala

Website : https://nextsoftwarethailand.com, https://autoworks24.com

Linkedin : https://linkedin.com/in/patasu-doungmala-7b90a2205

​
บริษัท เน็กซ์ ซอฟต์แวร์ จำกัด 

ที่อยู่ หมู่บ้าน inizio เลขที่ 888/257 ถนนมะลิวัลย์ ตำบลบ้านทุ่ม อำเภอเมืองขอนแก่น จังหวัดขอนแก่น 40000 เลขที่ผู้เสียภาษี : 0405558003118

ผลงานและประวัติการทำงาน

สามารถดูผลงานและประวัติการทำงานได้ที่

AI, Image Processing : https://www.dropbox.com/scl/fi/tskimhifw0hlcdea5e8t8/Next-Software-2026.pdf?rlkey=f26k2b7t69doklzwxyx54qsmh&dl=0

IoT : https://www.dropbox.com/scl/fi/a5mj4ucjotjv4xrh6sh9q/NS_IOT2025.pdf?rlkey=t0cwl0l4b81w73do2drhqqjp0&dl=0

SEO, Website : https://www.dropbox.com/scl/fi/4q811q0s88xtd8usf5e25/WEB-DEVELOPER-SEARCH-ENGINE-OPTIMIZATION.pdf?rlkey=nvqvndrxv7v9yrfmlcgtplmtx&dl=0

Affiliated companies : https://www.dropbox.com/scl/fi/y98k95g24x44511iyhdih/Affiliated-companies.pdf?rlkey=mf1z7lr6q5x58ee2nonmgnz8r&dl=0
