# 💼 Freelance Escrow & Smart Payment Platform

แพลตฟอร์มระบบจ้างงานฟรีแลนซ์แบบไร้ตัวกลางที่ใช้เทคโนโลยี Smart Contract บนเครือข่าย Ethereum (Sepolia Testnet) เพื่อทำหน้าที่เป็น Escrow ล็อคเงินค่าจ้างไว้ตรงกลาง ช่วยแก้ปัญหาผู้ว่าจ้างไม่จ่ายเงิน และฟรีแลนซ์ทิ้งงาน

🌐 **Live Demo (GitHub Pages):** [(https://github.com/Ratchawanlop/freelance-escrow-dapp)]

---

## 🛠 เทคโนโลยีที่ใช้งาน (Tech Stack)
* **Frontend:** HTML5, Tailwind CSS, JavaScript (Vanilla)
* **Web3 Library:** Ethers.js (v5.7.2)
* **Smart Contract:** Solidity (^0.8.0)
* **Network:** Sepolia Testnet

---

## 📋 สิ่งที่ต้องเตรียมก่อนใช้งาน (Prerequisites)
1. ติดตั้ง Web Extension [MetaMask](https://metamask.io/)
2. สมัครกระเป๋าและเปิดใช้งานเครือข่าย **Sepolia test network**
3. เตรียมเหรียญ SepoliaETH สำหรับใช้ทดสอบธุรกรรม (ขอฟรีได้จาก Faucet)
4. เตรียมกระเป๋า (Account) จำนวน 2 บัญชีใน MetaMask เพื่อจำลองเป็น **ผู้ว่าจ้าง (Employer)** และ **ฟรีแลนซ์ (Freelancer)**

---

## 🚀 วิธีการทดสอบระบบ (How to test)

### ขั้นตอนที่ 1: การฝากเงิน (ฝั่งผู้ว่าจ้าง)
1. สลับบัญชี MetaMask ไปที่กระเป๋าของ **ผู้ว่าจ้าง**
2. คัดลอก Contract Address ของโปรเจกต์มาวางในช่อง `Contract Address ที่ Deploy แล้ว`
3. กดปุ่ม **เชื่อมต่อ MetaMask**
4. ในกรอบ "ฝั่งผู้ว่าจ้าง" ให้กดปุ่ม **ฝากเงินค่าจ้างเข้า Escrow (Deposit)**
5. กดยืนยัน (Confirm) ธุรกรรมใน MetaMask และรอจนกว่าระบบจะแจ้งเตือนว่าฝากเงินสำเร็จ

### ขั้นตอนที่ 2: การส่งมอบงาน (ฝั่งฟรีแลนซ์)
1. สลับบัญชี MetaMask ไปที่กระเป๋าของ **ฟรีแลนซ์**
2. กดรีเฟรชหน้าเว็บ 1 ครั้ง (เพื่อดึง Address ใหม่) และกด **เชื่อมต่อ MetaMask**
3. ในกรอบ "ฝั่งฟรีแลนซ์" ให้นำลิงก์ผลงาน (เช่น ลิงก์ Google Drive, GitHub หรือ URL เว็บไซต์) มาใส่ในช่อง
4. กดปุ่ม **ส่งมอบงาน (Submit Work)** และกดยืนยันธุรกรรมใน MetaMask

### ขั้นตอนที่ 3: การตรวจรับและจ่ายเงิน (ฝั่งผู้ว่าจ้าง)
1. สลับบัญชี MetaMask กลับมาที่กระเป๋าของ **ผู้ว่าจ้าง**
2. กดรีเฟรชหน้าเว็บและกด **เชื่อมต่อ MetaMask** อีกครั้ง
3. กดปุ่ม **ตรวจรับงานและอนุมัติเงิน (Approve)**
4. กดยืนยันธุรกรรมใน MetaMask เมื่อธุรกรรมสำเร็จ Smart Contract จะทำการโอนเหรียญ SepoliaETH ทั้งหมดไปให้กระเป๋าของฟรีแลนซ์โดยอัตโนมัติ

---

## 📄 ข้อมูล Smart Contract (อ้างอิง)
* **Network:** Sepolia Testnet
* **Contract Address:** `0xFe2f5881d47D28DE97b44C1478A5b0CE64B71F93`
