<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NUREKE.KZ - Білім платформасы</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
</head>
<body>
    <header>
        <h1>NUREKE.KZ</h1>
        <p>Оқушыларға арналған оқу платформасы</p>
    </header>
    <main>
        <h2>Сыныпты таңдаңыз:</h2>
        <div class="grades">
            <div class="grade"><button onclick="openMaterials(1)">1-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(2)">2-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(3)">3-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(4)">4-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(5)">5-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(6)">6-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(7)">7-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(8)">8-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(9)">9-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(10)">10-сынып</button></div>
            <div class="grade"><button onclick="openMaterials(11)">11-сынып</button></div>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 NUREKE.KZ. Барлық құқықтар қорғалған.</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f9f9f9;
    color: #333;
}
header {
    background-color: #007bff;
    color: white;
    text-align: center;
    padding: 10px 0;
}
main {
    padding: 20px;
    text-align: center;
}
.grades {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}
.grade {
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 20px;
    width: 150px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: center;
}
.grade button {
    text-decoration: none;
    color: #007bff;
    font-weight: bold;
    background: none;
    border: none;
    cursor: pointer;
}
.grade button:hover {
    color: #0056b3;
}
footer {
    background-color: #f1f1f1;
    text-align: center;
    padding: 10px;
}
function openMaterials(grade) {
    const materials = {
        1: { book: "materials/book1/index.html", test: "materials/test1/index.html" },
        2: { book: "materials/book2/index.html", test: "materials/test2/index.html" },
        3: { book: "materials/book3/index.html", test: "materials/test3/index.html" },
        4: { book: "materials/book4/index.html", test: "materials/test4/index.html" },
        5: { book: "materials/book5/index.html", test: "materials/test5/index.html" },
        6: { book: "materials/book6/index.html", test: "materials/test6/index.html" },
        7: { book: "materials/book7/index.html", test: "materials/test7/index.html" },
        8: { book: "materials/book8/index.html", test: "materials/test8/index.html" },
        9: { book: "materials/book9/index.html", test: "materials/test9/index.html" },
        10: { book: "materials/book10/index.html", test: "materials/test10/index.html" },
        11: { book: "materials/book11/index.html", test: "materials/test11/index.html" },
    };

    if (materials[grade]) {
        window.open(materials[grade].book, '_blank');
        window.open(materials[grade].test, '_blank');
    } else {
        alert("Материалдар табылмады!");
    }
}
<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <title>1-сынып Кітабы</title>
</head>
<body>
    <h1>1-сынып кітаптары</h1>
    <ul>
        <li><a href="book1_file1.pdf" target="_blank">Кітап 1</a></li>
        <li><a href="book1_file2.pdf" target="_blank">Кітап 2</a></li>
    </ul>
</body>
</html>
<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <title>1-сынып Тесттері</title>
</head>
<body>
    <h1>1-сынып тесттері</h1>
    <ul>
        <li><a href="test1_file1.pdf" target="_blank">Тест 1</a></li>
        <li><a href="test1_file2.pdf" target="_blank">Тест 2</a></li>
    </ul>
</body>
</html>
