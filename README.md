# app8-1

โปรเจกต์ตัวอย่างการใช้งาน REST API ด้วย React (frontend) และ Express (backend)

## โครงสร้างโปรเจกต์

```
app8-1/
├── local/       # React frontend (Create React App)
└── server/      # Express backend
```

## การติดตั้ง

### Backend (server)

```bash
cd server
npm install
```

### Frontend (local)

```bash
cd local
npm install
```

## การรัน

เปิด 2 terminal แล้วรันแต่ละส่วนพร้อมกัน

### รัน Backend

```bash
cd server
npm start
```

Server จะรันที่ `http://localhost:8000`

### รัน Frontend

```bash
cd local
npm start
```

React app จะรันที่ `http://localhost:3000`

> Frontend ถูกตั้งค่า proxy ไปยัง `http://localhost:8000` ไว้แล้วใน `local/package.json`

## API Endpoints

| Method | Path | คำอธิบาย |
|--------|------|----------|
| `POST` | `/api/form-post` | รับข้อมูลฟอร์ม (name, email, message) แล้วส่งกลับเป็น HTML table |
| `GET`  | `/api/form-get`  | รับ query string (target, kw) แล้วส่งกลับผลลัพธ์แบบสุ่ม |
| `GET`  | `/api/server-time` | ส่งกลับเวลาปัจจุบันของ server |
| `GET`  | `/api/football-result` | ส่งกลับผลบอลแบบสุ่มเป็น HTML table |

## Tech Stack

- **Frontend**: React 19, Create React App
- **Backend**: Node.js, Express 5, Nodemon
