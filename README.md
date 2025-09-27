# Exam-Time-table-Alerts
Exam with alerts
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Exam Alert Login</title>
  <script src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
  <script>
    (function() {
      emailjs.init("L-LBoNsMxZDkAluk5");
    })();
  </script>
</head>
<body style="margin:0; font-family:Arial, sans-serif; display:flex; justify-content:center; align-items:center; height:100vh; background:#f4f4f9;">

  <!-- Login Section -->
  <div id="loginPage" class="container" 
       style="display:flex; justify-content:center; align-items:center; width:100%; height:100%;">
    <form class="card" onsubmit="return goToDashboard()" 
          style="background:#fff; padding:30px; border-radius:10px; box-shadow:0 4px 8px rgba(0,0,0,0.1); display:flex; flex-direction:column; gap:15px; width:300px; text-align:center;">
      <h2 style="margin:0; color:#333;">Aditya Exam Alert Login</h2>
      <input type="text" id="loginName" placeholder="Enter your name" required
