ภาพรวมโค้ด

# MainActivity.kt
- StudentApp: มี ViewModel และ isShowDialog เพื่อติดตามว่า Dialog สำหรับเพิ่มข้อมูลควรแสดงหรือไม่ เมื่อ Dialog ถูกเรียกใช้จะมีการส่ง viewModel เข้าไปใน isShowDialog ถูกปรับเปลี่ยนเพื่อปิด Dialog เมื่อมีการเพิ่มนักศึกษาสำเร็จ. 
- InputDialog: ใช้สร้าง Dialog สำหรับเพิ่มข้อมูลนักศึกษา.
- AppPreview: ใช้สร้างตัวอย่างของแอปพลิเคชันโดยใช้ StudentTheme

# StudentModel.kt

data class ใน Kotlin มักถูกใช้เพื่อทำให้ง่ายต่อการสร้างและใช้งานข้อมูลที่มีโครงสร้างคงที่
data class ที่ชื่อ StudentModel ใช้เก็บข้อมูล 
เช่น id แทนรหัสนศ. , name เป็นสตริงแทนชื่อนศ. , studentId เป็นสตริงแทนรหัสนศ.

# StudentViewModel.kt


ViewModel สำหรับแอปพลิเคชันที่ใช้ในการจัดการข้อมูล 
โดยมีฟังก์ชั่น addStudent ที่ใช้ในการเพิ่มข้อมูลในลิสต์ของข้อมูล (data).
