myYa — ไฟล์เพิ่มสำหรับ Repository เดิม

อัปโหลด index.html, pos.html, admin.html ไปที่ root ของ Repository (ระดับเดียวกับ dashboard.html และ status.html)
ห้ามลบหรือทับไฟล์ dashboard.html, drug_dashboard.html, status.html และโฟลเดอร์ api/

ไฟล์ pos.html ใช้ GET /api/data และ POST /api/dispense
ไฟล์ admin.html ใช้ GET /api/data และ POST /api/admin
ไฟล์ index.html เชื่อมไปยัง pos.html, admin.html, dashboard.html และ status.html

หลัง Commit ให้รอ Vercel Deploy สำเร็จ จากนั้นเปิด /index.html, /pos.html, /admin.html
ไฟล์ README นี้ไม่จำเป็นต้องอัปโหลด

การทดสอบขายจริงเปลี่ยนฐานข้อมูล Supabase ให้ใช้ข้อมูลจำลองและเตรียม reset ก่อน
ถ้า API ใช้ rewrite หรือ authentication พิเศษ ต้องตรวจ deployment บน Vercel อีกครั้ง
