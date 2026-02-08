# naman-sharma58
this is my 15th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zomato Style UI</title>
    <style>
        :root {
            --zomato-red: #ef4f5f;
            --text-dark: #1c1c1c;
            --text-gray: #828282;
            --bg-gray: #f8f8f8;
            --border: #e8e8e8;
        }

        body {
            font-family: 'Okra', Helvetica, sans-serif;
            background-color: white;
            margin: 0;
            padding: 20px;
        }

        /* Top Filter Bar */
        .filter-bar {
            display: flex;
            gap: 10px;
            margin-bottom: 25px;
            max-width: 1100px;
            margin-left: auto;
            margin-right: auto;
        }

        .filter-item {
            padding: 8px 12px;
            border: 1px solid var(--border);
            border-radius: 8px;
            color: var(--text-gray);
            font-size: 14px;
            cursor: pointer;
            background: white;
        }

        /* Restaurant Grid */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(330px, 1fr));
            gap: 30px;
            max-width: 1100px;
            margin: 0 auto;
        }

        /* Restaurant Card */
        .card {
            padding: 10px;
            border-radius: 15px;
            transition: transform 0.2s, box-shadow 0.2s;
            cursor: pointer;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            border: 1px solid var(--border);
        }

        .img-container {
            position: relative;
            width: 100%;
            height: 200px;
            border-radius: 15px;
            overflow: hidden;
            background-color: #eee;
        }

        .img-container iframe {
            width: 100%;
            height: 100%;
            border: none;
        }

        .promo-tag {
            position: absolute;
            bottom: 10px;
            left: 0;
            background-color: #256fef;
            color: white;
            padding: 2px 8px;
            font-size: 12px;
            font-weight: bold;
        }

        /* Details */
        .details {
            margin-top: 12px;
        }

        .row-one {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 5px;
        }

        .name { font-size: 18px; font-weight: 600; color: var(--text-dark); }
        
        .rating {
            background-color: #24963f;
            color: white;
            padding: 2px 5px;
            border-radius: 6px;
            font-size: 13px;
            font-weight: bold;
        }

        .row-two {
            display: flex;
            justify-content: space-between;
            color: var(--text-gray);
            font-size: 14px;
        }
    </style>
</head>
<body>

    <div class="filter-bar">
        <div class="filter-item">Filters</div>
        <div class="filter-item">Rating: 4.0+</div>
        <div class="filter-item">Pure Veg</div>
        <div class="filter-item">Cuisines ▼</div>
    </div>

    <div class="grid">
        <div class="card">
            <div class="img-container">
                <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0&mute=1" allowfullscreen></iframe>
                <div class="promo-tag">60% OFF</div>
            </div>
            <div class="details">
                <div class="row-one">
                    <span class="name">The ABES Canteen</span>
                    <span class="rating">4.2 ★</span>
                </div>
                <div class="row-two">
                    <span>North Indian, Beverages</span>
                    <span>₹200 for one</span>
                </div>
            </div>
        </div>

        <div class="card">
            <div class="img-container">
                <iframe src="https://www.youtube.com/embed/377pxMNUTwo?controls=0&mute=1"></iframe>
            </div>
            <div class="details">
                <div class="row-one">
                    <span class="name">Dadri Delights</span>
                    <span class="rating">3.9 ★</span>
                </div>
                <div class="row-two">
                    <span>Street Food, Mithai</span>
                    <span>₹150 for one</span>
                </div>
            </div>
        </div>
    </div>

</body>
</html>
