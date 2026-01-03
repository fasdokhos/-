# 📘 دليل الأوامر المهمة - StudyPro Commands

هذا الملف يحتوي على جميع الأوامر التي تحتاجها لتشغيل وتعديل وإدارة المشروع.
This file contains all the commands you need to run, modify, and manage the project.

---

## 🚀 1. تشغيل المشروع (Running the Project)

### تشغيل السيرفر (Start Backend Server)
هذا هو الأمر الأساسي لتشغيل البرنامج.
Run this command from the main folder `StudyPro`:
```bash
node backend/server_final.js
```

### إنشاء رابط عام (Generate Public Link)
لجعل الموقع متاحاً للآخرين عبر الإنترنت.
To make the site accessible online:
```bash
npx localtunnel --port 8000
```
*(انسخ الرابط الذي يظهر لك، وكلمة المرور هي عادةً IP جهازك إذا طُلب ذلك)*

---

## 🛠️ 2. الصيانة والتطوير (Development & Maintenance)

### تنصيب المكتبات (Install Dependencies)
إذا قمت بنقل المشروع لجهاز جديد، نفذ هذه الأوامر أولاً:
If you move the project to a new device, run these first:

**للسيرفر (Backend):**
```bash
cd backend
npm install
cd ..
```

**للموقع (Frontend):**
```bash
cd frontend
npm install
cd ..
```

---

## 💾 3. النسخ الاحتياطي (Backup)

### ضغط الملفات المهمة (Zip Important Code)
لعمل نسخة مضغوطة من الكود المصدري فقط (بدون الملفات المؤقتة):
To archive important source code only:
```powershell
powershell -Command "Compress-Archive -Path backend/src, backend/server_final.js, frontend/src -DestinationPath StudyPro_Code_Backup.zip -Force"
```

---

## 📝 ملاحظات مهمة (Important Notes)
- تأكد دائماً أنك في المجلد الرئيسي `StudyPro` عند كتابة الأوامر.
- لإيقاف أي أمر (مثل السيرفر)، اضغط `Ctrl + C` في الـ Terminal.
