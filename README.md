# FinFlow PWA — คู่มือติดตั้งบน iOS

## วิธี Deploy ขึ้น GitHub Pages (ฟรี)

### ขั้นตอนที่ 1 — สร้าง GitHub Repository

1. เปิด [github.com](https://github.com) แล้วล็อกอิน (หรือสมัครฟรี)
2. กด **New repository** (มุมบนขวา)
3. ตั้งชื่อ: `finflow` (หรืออะไรก็ได้)
4. เลือก **Public**
5. กด **Create repository**

---

### ขั้นตอนที่ 2 — อัปโหลดไฟล์

1. ในหน้า repository ใหม่ กด **uploading an existing file**
2. ลาก **ทุกไฟล์และโฟลเดอร์** จากโฟลเดอร์ `finflow-pwa/` ขึ้นไป
   ```
   index.html
   manifest.json
   sw.js
   icons/
     icon-apple-touch.png
     icon-192.png
     icon-512.png
   ```
3. กด **Commit changes**

---

### ขั้นตอนที่ 3 — เปิด GitHub Pages

1. ใน repository กด **Settings** (แถบด้านบน)
2. เลือก **Pages** (เมนูซ้าย)
3. ตรง **Source** เลือก:
   - Branch: `main`
   - Folder: `/ (root)`
4. กด **Save**
5. รอ 1-2 นาที จะได้ URL เช่น:
   ```
   https://ชื่อuser.github.io/finflow/
   ```

---

### ขั้นตอนที่ 4 — ติดตั้งบน iPhone/iPad

1. เปิด **Safari** (ต้องใช้ Safari เท่านั้น Chrome ไม่ได้)
2. ไปที่ URL ของแอป เช่น `https://ชื่อuser.github.io/finflow/`
3. กด ไอคอน **Share** (กล่องมีลูกศรชี้ขึ้น)
4. เลือก **"Add to Home Screen"**
5. ตั้งชื่อ: `FinFlow` → กด **Add**

แอปจะปรากฏบน Home Screen พร้อมไอคอนสีม่วง ✅

---

## ฟีเจอร์ PWA ที่ได้รับ

| ฟีเจอร์ | สถานะ |
|---------|-------|
| ติดตั้งบน Home Screen | ✅ |
| เปิดแบบ Full Screen (ไม่มี Safari bar) | ✅ |
| ใช้งานออฟไลน์ (ไม่มีเน็ต) | ✅ |
| ข้อมูลถาวร (IndexedDB) | ✅ |
| ไอคอนแอปสวยงาม | ✅ |
| Status bar สีม่วง | ✅ |
| อัปเดตอัตโนมัติเมื่อออนไลน์ | ✅ |
| Voice Input (ไมค์) | ✅ Safari รองรับ |
| OCR สแกนสลิป | ✅ ต้องมีเน็ต |
| Export CSV/Excel | ✅ ผ่าน Share Sheet |

---

## หมายเหตุ

- **ข้อมูลเก็บบนเครื่อง** ไม่ส่งไป server ใดๆ
- **อัปเดตแอป**: แก้ไข `index.html` แล้วอัปโหลด GitHub ใหม่ แอปจะ refresh อัตโนมัติ
- **สำรองข้อมูล**: กด 📤 → สำรองข้อมูล → บันทึกไฟล์ .json ไว้

---

*FinFlow v8 — สร้างด้วย Claude (Cowork)*
