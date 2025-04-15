<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>สมัครสมาชิก | Fly88</title>
  <style>
    body {
      font-family: sans-serif;
      background: #e0f7fa;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 400px;
      margin: 40px auto;
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
    }
    h2 {
      text-align: center;
      color: #0277bd;
    }
    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }
    input, select {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      margin-top: 20px;
      width: 100%;
      padding: 12px;
      background-color: #0288d1;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0277bd;
    }
    @media (max-width: 480px) {
      .container {
        margin: 20px;
        padding: 15px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>สมัครสมาชิก</h2>
    <form action="register.php" method="POST">
      <label>ชื่อ</label>
      <input type="text" name="firstname" required />

      <label>นามสกุล</label>
      <input type="text" name="lastname" required />

      <label>เบอร์โทรศัพท์</label>
      <input type="tel" name="phone" pattern="[0-9]{10}" required />

      <label>ธนาคาร</label>
      <select name="bank" required>
        <option value="">-- เลือกธนาคาร --</option>
        <option value="kbank">กสิกรไทย</option>
        <option value="scb">ไทยพาณิชย์</option>
        <option value="bbl">กรุงเทพ</option>
        <option value="ktb">กรุงไทย</option>
        <!-- เพิ่มธนาคารอื่น ๆ ตามต้องการ -->
      </select>

      <label>เลขบัญชี</label>
      <input type="text" name="account_number" required />

      <label>รหัสผ่าน</label>
      <input type="password" name="password" required />

      <button type="submit">สมัครสมาชิก</button>
    </form>
  </div>
</body>
</html>
