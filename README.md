# MDAP-EX_01-Portfolio
## Date:28/04/25

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM:

## Index.html:
'''
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="style.css">
        <title>Portfolio</title>
    </head>
    <body class="body">
        <header>
            <h1 id="heading">Portfolio</h1>
            <nav class="nav">
                <a href="#home">Home</a>
                <a href="#skills">Skills</a>
                <a href="#contact">Contact</a>
            </nav>
        </header>
        
        <section id="home">
            <div id="greet">
                <H3>Hello! I Am Kamalesh</H3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime hic minima culpa praesentium.            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Omnis nobis deserunt expedita aut amet, nostrum autem repellat consequuntur laborum impedit dolores praesentium, debitis quis, numquam eligendi eveniet. Reprehenderit, eum quidem?
                </p>
            </div>
            <div id="info">
                <img src="kamalesh2.jpeg" width="400" height="400" alt="Kamalesh">
            </div>
        </section>
        
        <section id="skills">
            <h2>Skills</h2>
            <div class="skimg">
                <div>
                    <img src="cyber.jpeg" width="400" height="300" alt="Penetration Testing">
                    <p>Penetration Testing</p>
                </div>
                <div>
                    <img src="web.jpeg" width="400" height="300" alt="JS Developer">
                    <p>JS Developer</p>
                </div>
                <div>
                    <img src="block.jpeg" width="400" height="300" alt="Blockchain Analyst">
                    <p>Blockchain Analyst</p>
                </div>
            </div>
        </section>
        
        <section id="contact">
            <h2>Contact Me</h2>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
            
                <label for="contact">Contact Number:</label>
                <input type="tel" id="contact" name="contact" required pattern="[0-9]{10}" placeholder="Enter 10-digit number">
            
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
            
                <label for="address">Address:</label>
                <textarea id="address" name="address" rows="1" required></textarea>
            
                <button type="submit">Submit</button>
            </form>
        </section>
        
        <script src="script.js"></script>
    </body>
    </html>

'''
## Stye.css:
'''
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f8f9fa;
            color: #333;
        }
        
        header {
            background: #1a1a2e;
            color: white;
            padding: 20px 0;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        
        #heading {
            margin: 0;
            font-size: 32px;
            font-weight: 600;
        }
        
        .nav {
            margin-top: 10px;
            gap : 20px;
        }
        
        .nav a {
            color: white;
            margin: 0 20px;
            font-size: 18px;
            text-decoration: none;
            transition: color 0.3s ease-in-out;
        }
        
        
        
        #home {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 80px 10%;
            max-width: 1200px;
            margin: auto;
        }
        
        #greet {
            width: 50%;
            text-align: left;
            font-size: 20px;
            font-weight: 100;
            color: #222;
        }
        
        
        
        #info img {
            width: 100%;
            max-width: 350px;
            border-radius: 12px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        
        
        #skills {
            background: #fff;
            padding: 60px 10%;
        }
        
        h2 {
            font-size: 36px;
            margin-bottom: 20px;
            font-weight: 600;
        }
        
        .skimg {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }
        
        .skimg div {
            background: white;
            padding: 15px;
            text-align: center;
            border-radius: 12px;
            box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.1);
        }
        
        
        
        .skimg img {
            width: 100%;
            max-width: 400px;
            border-radius: 10px;
        }
        
        
        form {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 30px;
            border-radius: 12px;
        }
        
        input, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 16px;
            transition: border 0.3s ease-in-out;
        }
        
        input:focus, textarea:focus {
            border-color: #1a1a2e;
            outline: none;
        }
        
        button {
            background: #1a1a2e;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 8px;
            font-size: 18px;
        }

'''

## Script.js:
'''

     document.getElementById("contactForm").addEventListener("submit")
      {
      
      
          let name = document.getElementById("name");
          let contact = document.getElementById("contact");
          let email = document.getElementById("email");
          let address = document.getElementById("address");
          let phonePattern = /^[0-9]{10}$/;
          if (name === "" || contact === "" || email === "" || address === "") {
              alert("Please fill out all fields.");
              return;
          }
          if (!phonePattern.test(contact)) {
              alert("Please enter a valid 10-digit contact number.");
              return;
          }
          alert("Form submitted successfully!");
          document.getElementById("contactForm").reset();
          
      };
'''

## OUTPUT
![image](https://github.com/user-attachments/assets/bc3cbf99-2192-4a72-8d0f-ffc79329239b)
![image](https://github.com/user-attachments/assets/7622a437-d06e-4a64-8804-c29a2fa824d1)
![image](https://github.com/user-attachments/assets/4625d138-82ac-41a2-bc05-a35a92af85f0)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
