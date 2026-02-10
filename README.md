# Ex03 Places Around Me
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
```
image.html:
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SAVEETHA</title>
</head>

<body>

    <img src="{% static 'Screenshot 2025-09-29 113906.png'%}" usemap="#saveetha" height="800px" width="1500px">
    <map name="saveetha">

        <area shape="poly" coords="422,257,507,919,905,935,900,950" title="SIMATS clg " href="{% url 'simats' %}">

        <area shape="rect" coords="500,600,1600,1600" title="Saveetha medical clg " href="{% url 'med' %}">


        <area  shape="rect" coords="429,268,553,274" title="Saveetha eng clg" href="{% url 'sav' %}">


    </map>
</body>

</html>


saveetha.html :
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SAVEETHA ENG CLG </title>

    <style>
        img {
            border-radius: 40px;
        }

        body {
            background-color: rgb(239, 22, 177);
            color: rgb(4, 4, 4);
        }

        h1 {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }

        p{
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }
    </style>
</head>

<body>
    <center>


        <h1>
            SAVEETHA ENGINEERING COLLEGE
        </h1>

        <img src="{% static 'Screenshot 2025-09-30 142309.png'%}" height="400px" width="800px">


        <br>
        <p>
            Saveetha Engineering College (SEC), founded in 2001 by the Saveetha Medical and Educational Trust, is a reputed autonomous institution located in Thandalam, Chennai. The college is affiliated with Anna University and approved by the AICTE, offering a wide range of undergraduate, postgraduate, and doctoral programs across various engineering and management disciplines. SEC is accredited by NAAC and NBA, reflecting its commitment to quality education, research, and innovation. The institution emphasizes a holistic learning environment, blending academic rigor with practical exposure, supported by modern laboratories, digital libraries, well-equipped classrooms, hostels, and excellent sports and cultural facilities. Its scenic campus overlooking Chembarambakkam Lake provides a conducive atmosphere for learning and growth. SEC is recognized as a Scientific and Industrial Research Organization (SIRO) and actively promotes innovation and entrepreneurship among students. The college also has an impressive placement record, with over 300 companies visiting annually, offering high-paying job opportunities; top recruiters include TCS, Accenture, Infosys, Cognizant, and Wipro. The highest package has touched ₹34 LPA, while the average remains strong, ensuring students are industry-ready. With its focus on academic excellence, skill development, and character building, Saveetha Engineering College continues to be one of the preferred destinations for aspiring engineers in Tamil Nadu
        </p>
    </center>
</body>

</html>

medical.html:
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SAVEETHA MEDICAL COLLEGE</title>

    <style>
        img{
            border-radius: 40px;
        }
        body{
            background-color: aqua;
            color: rgb(4, 4, 4);
        }
        h1{
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }
        p{
            font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
        }
    </style>
</head>

<body>
   
    <center>

        <h1>
            SAVEETHA MEDICAL COLLEGE
        </h1>
       <img src="{% static 'Screenshot 2025-09-30 141940.png'%}" height="400px" width="800px" >
       <p>
        Saveetha Medical College, located at Thandalam near Chennai, is a constituent of Saveetha Institute of Medical and Technical Sciences (SIMATS), a deemed-to-be university. Established in 2008, it is one of the top private medical colleges in India and has been ranked 11th in the NIRF 2025 medical category. The college offers MBBS with 250 seats, along with postgraduate (MD/MS), super-speciality (DM/MCh), and doctoral programs. Admissions are strictly based on NEET-UG and NEET-PG scores, with counselling conducted through the Medical Counselling Committee (MCC). The annual MBBS fee is around ₹25 lakhs for Indian students, while PG fees vary depending on specialization. The associated teaching hospital has about 1600 beds and provides exposure to a wide range of clinical cases, equipped with modern facilities like robotic surgery, ECMO, and advanced digital labs. With strong research output, state-of-the-art infrastructure, and recognition at both national and international levels, Saveetha Medical College is considered one of the premier choices among private medical institutions, though its high fees remain a major consideration for prospective students
       </p>


    </center>


</body>

</html>

SIMATS.html:
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SIMATS</title>
    <style>
        img{
            border-radius: 40px;
        }

        body{
            background-color: blueviolet;

        }

        h1{
            font-family:sans-serif;
        }
        p{
             font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
        }

    </style>

</head>

<body>

    <center>

        <h1>
            SIMATS COLLEGE
        </h1>
        <img src="{% static 'Screenshot 2025-09-30 140456.png'%}" height="400px" width="800px">

        <P>
          Saveetha Institute of Medical and Technical Sciences (SIMATS), also known as Saveetha University, is a deemed-to-be university located in Thandalam, Chennai, Tamil Nadu. Established under the Saveetha Medical and Educational Trust, it began with Saveetha Dental College in 1988 and later expanded into diverse fields including medicine, engineering, law, pharmacy, management, nursing, physiotherapy, architecture, and allied health sciences. Declared a university in 2005, SIMATS is recognized for its modern teaching methods, advanced digital classrooms, international collaborations, and strong focus on research. Spread over 181 acres with state-of-the-art infrastructure, including hospitals, laboratories, seminar halls, and Wi-Fi enabled campuses, it provides comprehensive academic and practical training. Accredited with an “A++” grade by NAAC, its dental and medical colleges consistently rank among the top in India, reflecting its academic excellence and reputation.
        </P>


    </center>
</body>

</html>


```



# OUTPUT

![alt text](<Screenshot 2025-10-02 153048.png>)
![alt text](<Screenshot 2025-10-02 153206.png>)
![alt text](<Screenshot 2025-10-02 153220.png>)
![alt text](<Screenshot 2025-10-02 153235.png>)



# RESULT
The program for implementing image maps using HTML is executed successfully.
