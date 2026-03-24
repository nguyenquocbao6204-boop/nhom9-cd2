<?php
$members = [
    [
        "name" => "Nguyễn Văn A",
        "mssv" => "123456",
        "image" => "images/member1.jpg",
        "desc" => "Trưởng nhóm, phụ trách backend"
    ],
    [
        "name" => "Trần Thị B",
        "mssv" => "234567",
        "image" => "images/member2.jpg",
        "desc" => "Thiết kế giao diện"
    ],
    [
        "name" => "Lê Văn C",
        "mssv" => "345678",
        "image" => "images/member3.jpg",
        "desc" => "Frontend developer"
    ]
];
?>

<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>Trang chủ nhóm</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<h1>Giới thiệu thành viên nhóm</h1>

<div class="container">
    <?php foreach ($members as $member): ?>
        <div class="card">
            <img src="<?= $member['image'] ?>" alt="Ảnh">
            <h2><?= $member['name'] ?></h2>
            <p>MSSV: <?= $member['mssv'] ?></p>
            <p><?= $member['desc'] ?></p>
        </div>
    <?php endforeach; ?>
</div>

</body>
</html>
