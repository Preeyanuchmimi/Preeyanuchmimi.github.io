## Lab Disable Inheritance

![cf](1.png)

---

### โจทย์
ข้อมูลบุคลากรที่เป็นความลับถูกจัดเก็บไว้บนไฟล์เซิร์ฟเวอร์ **CorpFiles**  
ในไดเรกทอรีที่ใช้ร่วมกันชื่อว่า **Personnel**

คุณจำเป็นต้องกำหนดสิทธิ์การเข้าถึงแบบ **NTFS** สำหรับโฟลเดอร์นี้  
เพื่อให้ **เฉพาะผู้จัดการ (Managers)** เท่านั้นที่ได้รับอนุญาตให้เข้าถึงข้อมูลได้

---

## วิธีการ กำหนดสิทธิ์ Full Control ให้กับกลุ่ม Managers สำหรับโฟลเดอร์ D:\Personnel

---

### 1. เปิด File Explorer
![cf](3.png)

---

### 2. ไปที่ไดรฟ์ D คลิกขวาที่โฟลเดอร์ Personnel → เลือก Properties
![cf](4.png)

---

### 3. ไปที่แท็บ Security คลิกปุ่ม Edit
![cf](5.png)

---

### 4. คลิก Add
![cf](7.png)

---

### 5. พิมพ์ชื่อกลุ่ม Managers→ คลิก Check Names → OK
![cf](8.png)

---

### 6. เลือกกลุ่ม Managers ในช่อง Permissions ให้ติ๊ก Allow – Full control
![cf](11.png)

---

### 7. คลิก Apply → OK กด OK เพื่อปิดหน้าต่างทั้งหมด
![cf](12.png)

---


## วิธีการ Remove inherited permissions ที่โฟลเดอร์ D:\Personnel

---

### 1. เปิด File Explorer ไปที่ *D:* คลิกขวา โฟลเดอร์ Personnel → เลือก Properties
![cf](13.png)

---

### 2. ไปที่แท็บ Security คลิกปุ่ม Advanced
![cf](15.png)

---

### 3. ด้านบนจะเห็นคำว่า “Enable inheritance” (แปลว่า ตอนนี้มีการสืบทอดสิทธิ์อยู่)
คลิกปุ่ม Disable inheritance
![cf](16.png)

---

### 4. จะมีหน้าต่างถาม → เลือก Remove all inherited permissions from this object
![cf](18.png)

---


### 5. คลิก Apply คลิก OK → OK
![cf](19.png)

---
