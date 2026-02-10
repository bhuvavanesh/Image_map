# Ex04 Places Around Me
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
~~~
map.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Map</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #3a484a;
        }
       
</style>
</head>
<body>
    {% load static %}
    <h1 style="text-align: center; color: aliceblue;">Anna Nagar</h1>
    <h2 style="text-align: center; color: aliceblue;">PAVAN KALYAN P</h2>
    <h2 style="text-align: center; color: aliceblue;">(25010044) </h2>
    <img src="{% static 'map.png' %}" usemap="#image-map" alt="Map Image"  style="display: block;width: 100%; height: auto;">
 <map name="image-map">
    
    <area shape="rect" coords="786,387,902,420" title="vr" href="vr.html">
    <area shape="rect" coords="681,26,769,62" title="saravana" href="saravana.html">
    <area shape="rect" coords="524,300,720,350" title="hospital" href="hospital.html">
    <area shape="rect" coords="676,268,862,282" title="computer" href="computer.html">
    <area shape="rect" coords="845,492,994,521" title="theater" href="theatre.html">>
</body>
</html>


vr.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>VR Chennai</title>
  <style>
    body {
      font-family: Arial, sans-serif;
        margin: 0;
        
    }
    header {
       
      background-image: url('static/vr.png');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
      padding: 2em;
      text-align: center;
    }
    nav {
      background-color: #3aacee;
      overflow: hidden;
    }
    nav a {
      float: left;
      display: block;
      color: white;
      padding: 0.75em 1em;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #575757;
    }
    main {
      flex:1;
      padding: 2em;
    }
    footer {
       background-image:linear-gradient(to left, #5fb9ff, #daf4f8);
      text-align: center;
      padding: 20px;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <header>
    <h1>VR CHENNAI</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <main>
   
    <section style="font-family: Arial, sans-serif; line-height: 1.6; padding: 20px; background-color: #7cd3ff80;">
  <h1>VR Chennai</h1>
  <p>VR Chennai is a premier lifestyle destination in Anna Nagar, Chennai, offering shopping, dining, entertainment, and cultural experiences all under one roof.</p>

  <h2>🏢 Overview</h2>
  <ul>
    <li><strong>Location:</strong> Jawaharlal Nehru Road, Anna Nagar West, Chennai</li>
    <li><strong>Opened:</strong> June 18, 2018</li>
    <li><strong>Developer & Owner:</strong> Virtuous Retail</li>
    <li><strong>Size:</strong> Over 1 million sq ft of retail space across 6 floors</li>
  </ul>

  <h2>🛍️ Shopping & Brands</h2>
  <p>VR Chennai hosts 250+ stores, including:</p>
  <ul>
    <li><strong>Fashion:</strong> H&M, Zara, Levi’s, Nike, Adidas, Allen Solly</li>
    <li><strong>Beauty:</strong> MAC, Nykaa, Bath & Body Works, Kama Ayurveda</li>
    <li><strong>Electronics:</strong> Apple (Aptronix), Samsung, Dell, HP</li>
    <li><strong>Jewelry:</strong> Caratlane, Tanishq, Bluestone</li>
  </ul>

  <h2>🍽️ Dining & Restaurants</h2>
  <p>A wide range of cuisines is available, from fast food to fine dining:</p>
  <ul>
    <li>Burger King, KFC, McDonald's, Starbucks</li>
    <li>Indian: Anjappar, Kailash Parbat, Kaaraikudi</li>
    <li>Desserts: Krispy Kreme, Haagen Dazs, Belgian Waffle</li>
  </ul>

  <h2>🎬 Entertainment & Experiences</h2>
  <ul>
    <li><strong>PVR ICON Multiplex:</strong> A 10-screen luxury cinema with art deco interiors</li>
    <li><strong>The Hive:</strong> A 50,000 sq ft co-working space</li>
    <li><strong>Open-air amphitheater:</strong> Event spaces for live music and cultural events</li>
    <li><strong>Farmer’s Market:</strong> Every Sunday from 10 AM to 7 PM</li>
  </ul>

  <h2>🎨 Architecture & Design</h2>
  <ul>
    <li>Inspired by South Indian temple towers (gopurams) and Madras checks</li>
    <li>Features murals by artists from Cholamandal Artists’ Village</li>
    <li>Cultural motifs include Dashavatara and historical maps of South Indian dynasties</li>
  </ul>

  <h2>🌐 More Info</h2>
  <p>Visit the official site: <a href="https://vrchennai.com/" target="_blank">VR Chennai</a></p>
</section>
    <a href="map.html">Go to Map</a>
    
  </main>

  <footer>
    &copy; 2025 My Website. All rights reserved.
  </footer>

</body>
</html>


computer.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sree Computers</title>
  <style>
    body {
      font-family: Arial, sans-serif;
        margin: 0;
        
    }
    header {
       
      background-image: url('static/computer.png');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
      color: white;
      padding: 2em;
      text-align: center;
    }
    nav {
      background-color: #3aacee;
      overflow: hidden;
    }
    nav a {
      float: left;
      display: block;
      color: white;
      padding: 0.75em 1em;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #575757;
    }
    main {;
      padding: 2em;
    }
    footer {
       background-image:linear-gradient(to left, #5fb9ff, #daf4f8);
      text-align: center;
      padding: 20px;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <header>
    

    <h1>SREE COMPUTERS</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <main>
   <section style="font-family: Arial, sans-serif; line-height: 1.6; padding: 20px; background-color: #54afff60;">
  <h1>Sree Computers, Anna Nagar</h1>
  <p><strong>Sree Computers</strong> is a well-established electronics service center located in <strong>Welcome Colony, Anna Nagar West Extension, Chennai</strong>. Known for its reliable laptop and desktop repair services, it has built a reputation for professionalism and customer satisfaction.</p>

  <h2>🔧 Services Offered</h2>
  <ul>
    <li>Laptop screen repair and replacement</li>
    <li>Motherboard and processor diagnostics</li>
    <li>RAM and hard disk upgrades</li>
    <li>Operating system installation and antivirus setup</li>
    <li>Data recovery and mobile unlocking</li>
    <li>Sales of desktops, laptops, and accessories</li>
  </ul>

  <h2>📍 Location & Contact</h2>
  <ul>
    <li><strong>Address:</strong> No. 25/8, Opposite Roshini Chemicals, Welcome Colony, Anna Nagar West Extension, Chennai – 600101</li>
    <li><strong>Phone:</strong> +91 94441 51510 / +91 98409 51510</li>
    <li><strong>Website:</strong> <a href="https://www.sreecomputers.net/" target="_blank">sreecomputers.net</a></li>
    <li><strong>Hours:</strong> Opens at 10:00 AM</li>
  </ul>

  <h2>💼 Why Choose Sree Computers?</h2>
  <ul>
    <li>Over 15 years of experience in electronics repair and IT services</li>
    <li>Quick diagnostics and same-day service for many issues</li>
    <li>Affordable pricing and transparent service process</li>
    <li>Expert technicians with strong domain knowledge</li>
  </ul>

  <h2>🌐 Branches</h2>
  <ul>
    <li>Anna Nagar West Extension, Chennai</li>
    <li>Arumbakkam (Head Office)</li>
    <li>Kanchipuram</li>
    <li>Tiruttani</li>
  </ul>

  <p>Whether you're facing a hardware issue or need a quick upgrade, Sree Computers offers dependable solutions with a customer-first approach.</p>
</section>
  <a href="map.html">Go to Map</a>
</main>

  <footer>
    &copy; 2025 My Website. All rights reserved.
  </footer>

</body>
</html>

hospital.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>The Madras Medical Mission hospital</title>
  <style>
    body {
      font-family: Arial, sans-serif;
        margin: 0;
        
    }
    header {
       
      background-image: url('static/hospital.png');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
      color: white;
      padding: 2em;
      text-align: center;
    }
    nav {
      background-color: #3aacee;
      overflow: hidden;
    }
    nav a {
      float: left;
      display: block;
      color: white;
      padding: 0.75em 1em;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #575757;
    }
    main {;
      padding: 2em;
    }
    footer {
       background-image:linear-gradient(to left, #5fb9ff, #daf4f8);
      text-align: center;
      padding: 20px;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <header>
    

    <h1>The Madras Medical Mission Hospital</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <main>
  <section style="font-family: Arial, sans-serif; line-height: 1.6; padding: 20px; background-color: #549def93;">
  <h1>Madras Medical Mission Hospital, Chennai</h1>
  <p><strong>The Madras Medical Mission (MMM)</strong> is a leading tertiary care hospital in Chennai, known for its excellence in super-specialty healthcare and compassionate patient services.</p>

  <h2>🏥 Overview</h2>
  <ul>
    <li><strong>Founded:</strong> 1982 as a charitable society inspired by Bishop Zachariah Mar Dionysius</li>
    <li><strong>Location:</strong> 4-A, Dr. J. Jayalalitha Nagar, Mogappair, Chennai, Tamil Nadu 600037</li>
    <li><strong>Capacity:</strong> 300 beds, including 74 ICU beds and 16 CCU beds</li>
    <li><strong>Accreditations:</strong> ISO 9001:2015, NABH certified</li>
  </ul>

  <h2>🩺 Centers of Excellence</h2>
  <ul>
    <li>Institute of Cardiovascular Diseases</li>
    <li>Institute of Reproductive Medicine & Women’s Health</li>
    <li>Institute of Gastroenterology & Liver Diseases</li>
    <li>Institute of Kidney Diseases, Urology & Organ Transplantation</li>
  </ul>

  <h2>🌍 International Patient Care</h2>
  <p>MMM provides personalized services for international patients, including travel assistance, accommodation, and multilingual support. The hospital follows globally recognized clinical protocols for high-quality outcomes.</p>

  <h2>🎓 Education & Training</h2>
  <ul>
    <li>MMM College of Health Sciences</li>
    <li>MMM College of Nursing</li>
    <li>Fellowship programs in cardiology, reproductive medicine, and more</li>
  </ul>

  <h2>🕒 Visiting Hours</h2>
  <ul>
    <li><strong>Patient Rooms:</strong> 5:00 PM – 7:00 PM</li>
    <li><strong>CCU:</strong> 11:00 AM – 11:30 AM & 4:00 PM – 5:00 PM</li>
    <li><strong>ICUs:</strong> 6:30 PM – 7:30 PM</li>
  </ul>

  <h2>📞 Contact & More Info</h2>
  <ul>
    <li><strong>Phone:</strong> +91 90949 87777</li>
    <li><strong>Website:</strong> <a href="https://www.madrasmedicalmission.org.in/" target="_blank">madrasmedicalmission.org.in</a></li>
  </ul>
</section>
  <a href="map.html">Go to Map</a>
</main>

  <footer>
    &copy; 2025 My Website. All rights reserved.
  </footer>

</body>
</html>

saravana.html


<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Legend Saravana Stores</title>
  <style>
    body {
      font-family: Arial, sans-serif;
        margin: 0;
        
    }
    header {
       
      background-image: url('static/saravana.png');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
      color: white;
      padding: 4em;
      text-align: center;
    }
    nav {
      background-color: #3aacee;
      overflow: hidden;
    }
    nav a {
      float: left;
      display: block;
      color: white;
      padding: 0.75em 1em;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #575757;
    }
    main {;
      padding: 2em;
    }
    footer {
       background-image:linear-gradient(to left, #5fb9ff, #daf4f8);
      text-align: center;
      padding: 20px;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <header>
    

    <h1>SARAVANA STORES</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <main>
   <section style="font-family: Arial, sans-serif; line-height: 1.6; padding: 20px; background-color: #57c6fa75;">
  <h1>Saravana Stores, Chennai</h1>
  <p><strong>Saravana Stores</strong> is one of South India's largest and most iconic retail chains, headquartered in <strong>T. Nagar, Chennai</strong>. Known for its massive inventory, affordable pricing, and festive shopping atmosphere, it attracts thousands of shoppers daily.</p>

  <h2>🏬 Overview</h2>
  <ul>
    <li><strong>Founded:</strong> 1969 by Thiru Saravana Selvarathnam</li>
    <li><strong>Headquarters:</strong> Ranganathan Street, T. Nagar, Chennai</li>
    <li><strong>Branches:</strong> Multiple locations across Tamil Nadu including Purasawalkam, Chromepet, Porur, Madurai, Coimbatore, and Tirunelveli</li>
    <li><strong>Website:</strong> <a href="https://www.supersaravanastores.com" target="_blank">supersaravanastores.com</a></li>
  </ul>

  <h2>🛍️ What You’ll Find</h2>
  <ul>
    <li><strong>Textiles:</strong> Sarees, salwars, shirts, pants, kidswear, bridal collections</li>
    <li><strong>Jewelry:</strong> Gold, silver, and fashion jewelry</li>
    <li><strong>Electronics:</strong> TVs, refrigerators, washing machines, kitchen appliances</li>
    <li><strong>Home Needs:</strong> Furniture, kitchenware, bedding, decor</li>
    <li><strong>Cosmetics & Accessories:</strong> Perfumes, makeup, bags, watches</li>
  </ul>

  <h2>💰 Why It’s Popular</h2>
  <ul>
    <li>Unbeatable prices through bulk buying and direct sourcing</li>
    <li>Massive inventory across multiple floors</li>
    <li>Festive discounts during Diwali, Pongal, and wedding seasons</li>
    <li>Family-friendly shopping experience</li>
  </ul>

  <h2>🗣️ Reputation</h2>
  <p>Saravana Stores is often described as <em>“Chennai’s shopping powerhouse”</em>, praised for its variety, affordability, and vibrant atmosphere. Peak hours can be crowded, but the deals are worth it!</p>
</section>
  <a href="map.html">Go to Map</a>
</main>

  <footer>
    &copy; 2025 My Website. All rights reserved.
  </footer>

</body>
</html>

theatre.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Rohini silver screens</title>
  <style>
    body {
      font-family: Arial, sans-serif;
        margin: 0;
        
    }
    header {
       
      background-image: url('static/theatre.png');
      background-size: cover;
      background-repeat: no-repeat;
      background-position: center;
      color: white;
      padding: 6em;
      text-align: center;
    }
    nav {
      background-color: #3aacee;
      overflow: hidden;
    }
    nav a {
      float: left;
      display: block;
      color: white;
      padding: 0.75em 1em;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #575757;
    }
    main {;
      padding: 2em;
    }
    footer {
       background-image:linear-gradient(to left, #5fb9ff, #daf4f8);
      text-align: center;
      padding: 20px;
      bottom: 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <header>
    

    <h1>ROHINI SILVER SCREENS</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <main>
   <section style="font-family: Arial, sans-serif; line-height: 1.6; padding: 20px; background-color: #4fa9f380;">
  <h1>Rohini Silver Screens, Chennai</h1>
  <p><strong>Rohini Silver Screens</strong> is a legendary multiplex in Koyambedu, Chennai, known for its vibrant atmosphere, first-day-first-show culture, and immersive movie experience.</p>

  <h2>🎬 Overview</h2>
  <ul>
    <li><strong>Location:</strong> 141/2, Poonamallee High Road, Koyambedu, near St. Thomas College of Arts and Science, Chennai</li>
    <li><strong>Established:</strong> 1991</li>
    <li><strong>Milestone:</strong> Became India’s first 6-screen multiplex in 1999</li>
    <li><strong>Screens:</strong> 6, including the iconic Rohini Screen</li>
  </ul>

  <h2>🌟 What Makes It Special</h2>
  <ul>
    <li>First-Day-First-Show hub for Tamil cinema fans</li>
    <li>Electric atmosphere with fan celebrations and actor visits</li>
    <li>Affordable and unique snack options during special releases</li>
    <li>Easy access via Koyambedu Metro Station and ample parking</li>
  </ul>

  <h2>🔊 Experience & Features</h2>
  <ul>
    <li>High-quality screens with immersive sound</li>
    <li>Spacious seating and well-maintained interiors</li>
    <li>Festive decor during major releases</li>
  </ul>

  <h2>💡 Tips for Visitors</h2>
  <ul>
    <li>Book tickets early via <a href="https://in.bookmyshow.com/buytickets/rohini-silver-screens-koyambedu/cinema-chen-RSSC-MT/" target="_blank">BookMyShow</a></li>
    <li>Visit on weekdays or early shows for less crowd</li>
    <li>Explore nearby cafes and snack counters</li>
  </ul>

  <h2>🗣️ Reviews & Reputation</h2>
  <p>Rated highly by locals and tourists, with over 36,000 reviews praising its cinematic vibe and fan culture. Ranked among the top performing arts theatres in Chennai.</p>
</section>
    <a href="map.html">Go to Map</a>
  </main>

  <footer>
    &copy; 2025 My Website. All rights reserved.
  </footer>

</body>
</html>


~~~
# OUTPUT
<img width="1022" height="547" alt="Screenshot 2026-02-09 115008" src="https://github.com/user-attachments/assets/c42e6024-bdc5-42fb-a948-c148c74ad47d" />

<img width="1013" height="527" alt="Screenshot 2026-02-09 115016" src="https://github.com/user-attachments/assets/5b821632-0723-47ff-8e73-a92ba26486fa" />
<img width="1016" height="517" alt="Screenshot 2026-02-09 115023" src="https://github.com/user-attachments/assets/49ad3633-111a-4083-b531-6c322d8606e6" />

<img width="1013" height="404" alt="Screenshot 2026-02-09 115032" src="https://github.com/user-attachments/assets/419eb727-2983-4e77-be68-338808a726ba" />
<img width="1019" height="537" alt="Screenshot 2026-02-09 115044" src="https://github.com/user-attachments/assets/4e9b11eb-e2ec-4416-b281-35a1ec402e5c" />

# RESULT
The program for implementing image maps using HTML is executed successfully.
