# Exam-Time-table-Alerts
Exam with alerts
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Exam Alert Login</title>

  <!-- ✅ Internal CSS Starts Here -->
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f9;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
    }

    .card {
      background: white;
      width: 350px;
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    h2, h3, h4 {
      margin-bottom: 15px;
    }

    input {
      width: 90%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      width: 95%;
      background: #007BFF;
      border: none;
      color: white;
      padding: 10px;
      margin-top: 10px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
    }

    button:hover {
      background: #0056b3;
    }

    #pastExamList {
      list-style: none;
      padding: 0;
    }

    #pastExamList li {
      background: #eaeaea;
      margin: 5px 0;
      padding: 8px;
      border-radius: 5px;
    }
  </style>
  <!-- ✅ Internal CSS Ends Here -->

  <script src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
  <script>
    (function() {
      emailjs.init("L-LBoNsMxZDkAluk5");
    })();
  </script>
</head>
<body>

  <!-- Login Section -->
  <div id="loginPage" class="container">
    <form class="card" onsubmit="return goToDashboard()">
      <h2>Aditya Exam Alert Login</h2>
      <input type="text" id="loginName" placeholder="Enter your name" required />
      <button type="submit">Login</button>
    </form>
  </div>

  <!-- Dashboard Section -->
  <div id="dashboard" class="container" style="display: none;">
    <div class="card">
      <h2>📅 Exam Timetable with Email Alerts</h2>
      <h3 id="welcomeText"></h3>

      <form id="examForm">
        <input type="email" name="student_email" placeholder="Your Email" required />
        <input type="text" name="exam_name" placeholder="Exam Name" required />
        <input type="datetime-local" name="exam_time" required />
        <button type="submit">Set Email Alert</button>
      </form>

      <div id="pastExams">
        <h4>📋 Past Exams</h4>
        <ul id="pastExamList"></ul>
      </div>
    </div>
  </div>

  <script>
    function goToDashboard() {
      const name = document.getElementById("loginName").value.trim();
      if (!name) {
        alert("Please enter your name");
        return false;
      }

      document.getElementById("loginPage").style.display = "none";
      document.getElementById("dashboard").style.display = "flex";
      document.getElementById("welcomeText").innerText = `Welcome, ${name}`;
      return false;
    }

    function addPastExam(name, time) {
      const list = document.getElementById("pastExamList");
      const li = document.createElement("li");
      li.innerText = `${name} - ${new Date(time).toLocaleString()}`;
      list.prepend(li);
    }

    document.getElementById("examForm").addEventListener("submit", function(e) {
      e.preventDefault();

      const name = document.getElementById("welcomeText").innerText.replace("Welcome, ", "");
      const form = this;
      const formData = new FormData(form);
      const examName = formData.get("exam_name");
      const examTime = new Date(formData.get("exam_time"));
      const now = new Date();
      const delay = examTime - now;

      if (delay <= 0) {
        addPastExam(examName, examTime);
        alert("This exam time is already past.");
        return;
      }

      alert("Email alert scheduled!");

      setTimeout(() => {
        emailjs.send("service_yaf93qg", "template_29jbucr", {
          student_name: name,
          student_email: formData.get("student_email"),
          exam_name: examName,
          exam_time: formData.get("exam_time"),
        }).then(() => {
          alert("📧 Email sent successfully!");
        }, (error) => {
          alert("❌ Failed to send email: " + error.text);
        });
      }, delay);
    });
  </script>

</body>
</html>
