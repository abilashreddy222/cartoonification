# 🎨 Cartoonify Image Web App

The **Cartoonify Image Web App** is a simple and interactive web application that transforms normal photos into **cartoon-style images**.

The application is built using **Python, Flask, and OpenCV**. Users can upload an image through the web interface, and the system processes the image using computer vision techniques to generate a cartoon version.

The final cartoon image is displayed on the webpage and can also be **downloaded directly by the user*

---

# 🚀 Features

* Upload images directly from your device
* Convert images into cartoon-style artwork automatically
* Fast image processing using OpenCV
* Dark Mode / Light Mode interface
* Loading animation while the image is being processed
* Popup notification when the cartoon image is ready
* Preview the generated cartoon image on the page
* Download the cartoon image easily
* Responsive design that works on desktop and mobile devices

---

# 🛠️ Technologies Used

## Backend

* **Python** – Core programming language used to build the application
* **Flask** – Lightweight web framework used to create the web server and handle requests
* **OpenCV** – Computer vision library used for image processing
* **NumPy** – Used for handling image arrays and mathematical operations

## Frontend

* **HTML5** – Structure of the web page
* **CSS3** – Styling and layout
* **JavaScript** – Interactive features such as dark mode and loader animation

## Additional Libraries

* **Werkzeug** – Used for secure file uploads with `secure_filename()`

---

# 📂 Project Structure

```
cartoonify-project
│
├── app.py
│
├── static
│   ├── uploads      # Stores uploaded images temporarily
│   └── outputs      # Stores generated cartoon images
│
├── templates
│   └── index.html   # Main user interface
│
└── README.md
```

---

# ⚙️ Installation Guide

Follow these steps to run the project on your local machine.

### 1️⃣ Clone the Repository

```
git clone https://github.com/yourusername/cartoonify-project.git
cd cartoonify-project
```

### 2️⃣ Install Required Libraries

Install the dependencies using pip:

```
pip install flask opencv-python numpy werkzeug
```

### 3️⃣ Run the Application

Start the Flask server:

```
python app.py
```

---

# 🌐 Open the Application in Your Browser

Once the server is running, open your browser and go to:

```
http://127.0.0.1:5000
```

You will see the Cartoonify interface where you can upload an image and generate the cartoon version.

---

# 🧠 How the Application Works

The cartoonification process is performed using several **image processing techniques** provided by OpenCV.

Step-by-step process:

1. The user uploads an image through the web interface.
2. Flask receives the uploaded file and saves it temporarily.
3. The image is processed using OpenCV.
4. Several transformations are applied to create a cartoon effect.
5. The processed image is saved in the outputs folder.
6. The final cartoon image is displayed on the webpage.
7. The user can download the generated cartoon image.

---

# 📸 Image Processing Pipeline

The following steps are used to convert the original image into a cartoon image:

```
Original Image
      ↓
Convert Image to Grayscale
      ↓
Apply Median Blur (reduce noise)
      ↓
Detect Edges using Adaptive Threshold
      ↓
Apply Bilateral Filter (smooth colors)
      ↓
Combine Edges with Color Image
      ↓
Generate Cartoon Image
```

---

# 🔒 Security Considerations

The application includes basic security practices:

* Uploaded filenames are cleaned using **Werkzeug secure_filename**
* Files are processed locally on the server
* Images are not stored permanently beyond the processing stage

---

# 🎯 Future Improvements

Some features that can be added in future versions:

* Multiple cartoon styles and filters
* Drag and drop image upload
* Before / After comparison slider
* Real-time webcam cartoon filter
* Cloud deployment for public access
* Image history gallery

# ⭐ Support

If you like this project, please consider **starring the repository on GitHub**.
Your support helps the project grow and reach more developers.
