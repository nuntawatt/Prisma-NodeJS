# Node.js API with Prisma v7 + PostgreSQL

REST API พื้นฐานที่สร้างด้วย **Node.js**, **Express**, และ **Prisma ORM v7** โดยเก็บข้อมูลลงฐานข้อมูล **PostgreSQL** 

---
## Set env
```bash
DATABASE_URL="postgresql://username:password@localhost:5432/mydb?schema=public"
PORT=8000
```
---

## package.json
```bash
"scripts"
- เพิ่ม
"prisma:migrate": "prisma migrate dev",
"prisma:generate": "prisma generate"
```
---

## Initial Migration
```bash
npx prisma migrate dev --name init_user
```
---

## Update Table
- กรณีอัพเดท หรือเพิ่มTable
```bash
ืnpm run prisma:migrate
```
---

## Prisma Generate (กรณีต้องการ generate client ใหม่)
```bash
npm run prisma:generate