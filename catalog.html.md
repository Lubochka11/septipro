<!DOCTYPE html>  
<html lang="ru">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Каталог продуктов</title>  
    <style>  
        * { margin: 0; padding: 0; box-sizing: border-box; }  
        body { font-family: -apple-system, sans-serif; background: #f8f8f8; color: #222; padding: 20px; }  
        .container { max-width: 1200px; margin: 0 auto; }  
        h1 { font-size: 28px; margin-bottom: 20px; }  
        .search-bar { width: 100%; padding: 12px 16px; font-size: 16px; border: 1px solid #ddd; border-radius: 8px; margin-bottom: 20px; background: #fff; }  
        .categories { display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 30px; }  
        .category-btn { padding: 8px 18px; background: #fff; border: 1px solid #ddd; border-radius: 20px; cursor: pointer; font-size: 14px; }  
        .category-btn.active { background: #4caf50; color: #fff; border-color: #4caf50; }  
        .sort-bar { display: flex; gap: 10px; margin-bottom: 20px; align-items: center; }  
        .sort-btn { padding: 6px 14px; background: #fff; border: 1px solid #ddd; border-radius: 6px; cursor: pointer; font-size: 14px; }  
        .sort-btn.active { background: #333; color: #fff; }  
        .products-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 20px; }  
        .product-card { background: #fff; border-radius: 12px; overflow: hidden; box-shadow: 0 2px 8px rgba(0,0,0,0.05); cursor: pointer; }  
        .product-card img { width: 100%; height: 160px; object-fit: cover; background: #f5f5f5; }  
        .product-info { padding: 15px; }  
        .product-info h3 { font-size: 15px; font-weight: 500; margin-bottom: 4px; line-height: 1.3; }  
        .product-info .weight { font-size: 13px; color: #888; margin-bottom: 10px; }  
        .product-info .price { font-size: 20px; font-weight: 700; margin-bottom: 12px; }  
        .add-btn { width: 100%; padding: 10px; background: #4caf50; color: #fff; border: none; border-radius: 8px; font-size: 15px; cursor: pointer; }  
        @media (max-width: 600px) { .products-grid { grid-template-columns: repeat(2, 1fr); gap: 10px; } }  
    </style>  
</head>  
<body>  
<div class="container">  
    <h1>Каталог</h1>  
    <input type="text" class="search-bar" placeholder="Поиск по товарам...">  
    <div class="categories">  
        <button class="category-btn active">Все</button>  
        <button class="category-btn">Молочное</button>  
        <button class="category-btn">Сыры</button>  
        <button class="category-btn">Хлеб</button>  
        <button class="category-btn">Мясо</button>  
        <button class="category-btn">Овощи и фрукты</button>  
        <button class="category-btn">Бакалея</button>  
        <button class="category-btn">Бытовая химия</button>  
    </div>  
    <div class="sort-bar">  
        <span>Сортировка:</span>  
        <button class="sort-btn active">По цене ↑</button>  
        <button class="sort-btn">По цене ↓</button>  
        <button class="sort-btn">По названию</button>  
    </div>  
    <div class="products-grid">  
        <div class="product-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='200'%3E%3Crect fill='%23f5f5f5' width='300' height='200'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%23999' font-size='16'%3EМолоко Простоквашино%3C/text%3E%3C/svg%3E" alt=""><div class="product-info"><h3>Молоко Простоквашино 2.5%</h3><p class="weight">950 мл</p><p class="price">от 73₽</p><button class="add-btn">Добавить</button></div></div>  
        <div class="product-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='200'%3E%3Crect fill='%23f5f5f5' width='300' height='200'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%23999' font-size='16'%3EТворог Простоквашино%3C/text%3E%3C/svg%3E" alt=""><div class="product-info"><h3>Творог Простоквашино 5%</h3><p class="weight">200 г</p><p class="price">от 66₽</p><button class="add-btn">Добавить</button></div></div>  
        <div class="product-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='200'%3E%3Crect fill='%23f5f5f5' width='300' height='200'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%23999' font-size='16'%3EСметана Простоквашино%3C/text%3E%3C/svg%3E" alt=""><div class="product-info"><h3>Сметана Простоквашино 20%</h3><p class="weight">300 г</p><p class="price">от 58₽</p><button class="add-btn">Добавить</button></div></div>  
        <div class="product-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='200'%3E%3Crect fill='%23f5f5f5' width='300' height='200'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%23999' font-size='16'%3EЯйца Окское%3C/text%3E%3C/svg%3E" alt=""><div class="product-info"><h3>Яйца Окское С0</h3><p class="weight">10 шт</p><p class="price">от 89₽</p><button class="add-btn">Добавить</button></div></div>  
        <div class="product-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='200'%3E%3Crect fill='%23f5f5f5' width='300' height='200'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%23999' font-size='16'%3EМасло Вкуснотеево%3C/text%3E%3C/svg%3E" alt=""><div class="product-info"><h3>Масло Вкуснотеево 82.5%</h3><p class="weight">180 г</p><p class="price">от 166₽</p><button class="add-btn">Добавить</button></div></div>  
        <div class="product-card"><img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='200'%3E%3Crect fill='%23f5f5f5' width='300' height='200'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' fill='%23999' font-size='16'%3EСыр Ламбер%3C/text%3E%3C/svg%3E" alt=""><div class="product-info"><h3>Сыр Ламбер 50%</h3><p class="weight">200 г</p><p class="price">от 183₽</p><button class="add-btn">Добавить</button></div></div>  
    </div>  
</div>  
</body>  
</html>  
