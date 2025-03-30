[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/OspoeYOK)

วิธีการติดตั้งและรันโค้ด (How to Install and Run the Code)

1.ดาวน์โหลดโฟลเดอร์ sec2_gr6_fe_src และ sec2_gr6_ws_src และนำทั้งสองโฟลเดอร์ไปใส่โฟลเดอร์ใหม่อีกโฟลเดอร์หนึ่ง(ตั้งชื่อโฟลเดอร์นั้นว่าอะไรก็ได้) และนำโฟลเดอร์ใหม่ที่สร้างขึ้นไปเปิดใน vscode
ดังนั้น path file จำเป็นต้องเป็นลักษณะดังนี้ (1.Download the folders sec2_gr6_fe_src and sec2_gr6_ws_src, and place both folders into a new folder (you can name the folder anything you like). Then, open this newly created folder in VSCode.)

![image](https://github.com/user-attachments/assets/941032a0-d46d-47a9-b76b-07cffce5c26a)

2.ทำการดาวน์โหลด secX_grY_database.sql ลงเครื่อง (2.Download the secX_grY_database.sql file to your computer.)

![image](https://github.com/user-attachments/assets/00bed08a-cd25-4fab-b46b-d0cd0fb3b44b)

จากภาพ ให้ทำการรันบรรทัดที่ 7-8 ก่อน จึงค่อยรันบรรทัดที่ 1-4 จากนั้นรันทุกบรรทัดที่ไม่ได้มีการ comment ไว้ (From the image, run lines 7-8 first, then run lines 1-4. After that, run all the lines that are not commented out.)

3.ทำการเชื่อมต่อ sql database กับ user โดย grant all privileges on sec2_gr6_database.* to '{ชื่อ user}'@'localhost'; (ให้ user ดังกล่าวมี from host เป็น localhost)
(3.Connect to the SQL database with the user by using the following command: GRANT ALL PRIVILEGES ON sec2_gr6_database.* TO '{username}'@'localhost'; )

4.ในไฟล์ .env ดังรูป ให้เปลี่ยนข้อมูล DB_user และ DB_pass เป็นของผู้ใช้ (In the .env file as shown in the image, change the DB_user and DB_pass values to the user's credentials.)

![image](https://github.com/user-attachments/assets/9e82eceb-25bc-404f-a11c-bf087ad25f38)
![image](https://github.com/user-attachments/assets/718bd6c0-dc50-4663-98ee-74b6227aedde)

5.ในโปรแกรม vscode เมื่อ path file เป็นไปตามดังรูปข้อที่ 1 แล้ว ให้ทำการ new terminal และแบ่ง terminal เป็นสองส่วน จากนั้น ในแต่ละฝั่งของ terminal ให้พิมพ์คำสั่งดังรูป
(5.In VSCode, once the file path is set according to the instructions in step 1, create a new terminal and split the terminal into two sections. Then, in each terminal section, type the commands as shown in the image.)

![image](https://github.com/user-attachments/assets/f3c23e29-5a8b-42a2-af67-6265a6c292a0)


และคำสั่งถัดมาให้พิมพ์ npm start (And the next command to type is npm start.)

นี่คือผลลัพธ์หลังจาก npm start (This is result after 'npm start')

![image](https://github.com/user-attachments/assets/d7efe53e-d6c0-4698-9ede-859f80cc8523)


6.ให้ทำการไปที่เว็บบราวเซอร์และพิมพ์ localhost:3030/{หน้าที่ต้องการ เช่น homepage} และทำการทดสอบ (Go to your web browser and type localhost:3030/{the page you want, e.g., homepage} and perform the testing.)
![image](https://github.com/user-attachments/assets/3f8cd5e9-d666-4855-9f9e-532957b8b8f7)


Note: หากมีการทดสอบหน้าที่ต้องเพิ่ม/อัพเดท/ลบข้อมูล และมี error เกิดขึ้นเช่น มีการเพิ่ม PRIMARY KEY ที่ซ้ำ ทั้งที PRIMARY KEY นั้นไม่มีอยู่จริง กรุณาทำการรีโหลดโปรแกรม mysql
(Note: If you are testing a page that requires adding, updating, or deleting data and encounter an error (such as trying to add a duplicate PRIMARY KEY even though the PRIMARY KEY does not exist), please reload the MySQL program.)



