## Exercise_1
# วิธีการทำนะครับ
1.เข้า App Script แล้วกดที่ new project

![Screenshot 2024-12-02 061140](https://github.com/user-attachments/assets/acbb3096-3efb-4fb7-adc6-8d3a77585254)

2.พอเข้ามาได้แล้วจะได้หน้านี้นะครับ

![Screenshot 2024-12-02 061140](https://github.com/user-attachments/assets/2709c051-95c6-47ab-bf09-9fc4b5fbd4a4)

3.ให้เราไปเปลี่ยนชื่อเป็นชื่อ เลขที่_ชื่อนักเรียน_exercise1

![git2](https://github.com/user-attachments/assets/82c72eb5-e7a4-4e34-a88d-25ea62f72c54)


4.หลังจากนั้นให้นักเรียนสร้างไฟล์ โดยกดเครื่องหมาย + ดังภาพ

![git1](https://github.com/user-attachments/assets/add3c777-ddae-4fbe-bf2c-8128ce672de8)


แล้วเลื่อก HTML 

![4](https://github.com/user-attachments/assets/b174af28-59d6-45e6-9fc1-0fb22edbc9d4)

แล้วตั้งชื่อไฟล์ให้ชื่อ index
หลังจากนั้นเราจะได้ไฟล์ index.html

5.หลังจากนั้นให้เราเข้าไปแก้ไขไฟล์โดยใช้ code ตามตัวอย่าง

![6](https://github.com/user-attachments/assets/dc922b1b-f902-40f5-8c75-af828bc5b43e)

# อันนี้คือตัว code

-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Object Fit Practice</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
      color: #333;
    }

    h1 {
      text-align: center;
      margin-top: 20px;
      font-size: 2rem;
      color: #444;
    }

    div {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 20px;
    }

    div > div {
      width: 250px;
      text-align: center;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      background-color: #fff;
      padding: 10px;
    }

    img {
      width: 100%;
      height: 200px;
      border-radius: 8px;
      margin-bottom: 10px;
    }

    p {
      font-size: 0.9rem;
      color: #555;
    }

    strong {
      font-weight: bold;
      color: #333;
    }
  </style>
</head>
<body>
  <h1>Object Fit Practice</h1>
  <div>
    <div>
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSIbcr8qdAn6Fv0GaPrq8z-X1XZR5vjkNHXiQ&s" style="object-fit: fill;" alt="Object Fit Fill">
      <p><strong>object-fit: fill;</strong><br>ภาพจะถูกยืดหรือบีบให้เต็มกรอบโดยไม่รักษาสัดส่วน</p>
    </div>
    <div>
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSIbcr8qdAn6Fv0GaPrq8z-X1XZR5vjkNHXiQ&s" style="object-fit: contain;" alt="Object Fit Contain">
      <p><strong>object-fit: contain;</strong><br>ภาพจะถูกปรับให้พอดีกับกรอบโดยรักษาสัดส่วน</p>
    </div>
    <div>
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSIbcr8qdAn6Fv0GaPrq8z-X1XZR5vjkNHXiQ&s" style="object-fit: cover;" alt="Object Fit Cover">
      <p><strong>object-fit: cover;</strong><br>ภาพจะถูกขยายให้เต็มกรอบโดยรักษาสัดส่วน แต่บางส่วนอาจถูกครอบตัด</p>
    </div>
    <div>
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSIbcr8qdAn6Fv0GaPrq8z-X1XZR5vjkNHXiQ&s" style="object-fit: none;" alt="Object Fit None">
      <p><strong>object-fit: none;</strong><br>ภาพจะแสดงตามขนาดจริงโดยไม่ปรับให้พอดีกับกรอบ</p>
    </div>
    <div>
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSIbcr8qdAn6Fv0GaPrq8z-X1XZR5vjkNHXiQ&s" style="object-fit: scale-down;" alt="Object Fit Scale-down">
      <p><strong>object-fit: scale-down;</strong><br>ภาพจะถูกปรับขนาดเล็กที่สุดระหว่าง none และ contain</p>
    </div>
  </div>
</body>
</html>

6.เข้าไปแก้ในไฟล์ code.gs

![7](https://github.com/user-attachments/assets/43913c94-ee6a-40cc-980d-758442e2fe32)

# อันนี้คือ code ของ code.gs

function doGet() {
    return HtmlService.createHtmlOutputFromFile('index');
}

หลังจากนั้นก็กด deploy
