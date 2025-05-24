<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
</head>
<body>

  <h1>🚀 CI/CD Pipeline: Deploy Flask App to EC2 with GitHub Actions</h1>

  <p>This project demonstrates a complete CI/CD pipeline setup to deploy a Flask application to an AWS EC2 instance using GitHub Actions, SSH, and PM2. It covers secure key-based authentication, auto-deployment from GitHub, process management with PM2, and firewall setup.</p>

  <h2>📦 Project Overview</h2>
  <ul>
    <li>Create a simple Flask app (<code>app.py</code>)</li>
    <li>Launch an AWS EC2 Ubuntu instance</li>
    <li>Set up SSH key pair and configure GitHub Secrets</li>
    <li>Install and configure PM2 on the EC2 server</li>
    <li>Create a GitHub Actions workflow (<code>.github/workflows/deploy.yml</code>)</li>
    <li>Enable firewall rules for SSH and app access (e.g., port 5000)</li>
    <li>Deploy on every push to <code>main</code></li>
  </ul>

  <h2>🛠️ Technologies Used</h2>
  <ul>
    <li>Python + Flask</li>
    <li>GitHub Actions (CI/CD)</li>
    <li>AWS EC2 (Ubuntu)</li>
    <li>PM2 (Process Manager)</li>
    <li>SSH Key Authentication</li>
  </ul>

  <h2>🧪 Deployment Workflow</h2>
  <ol>
    <li>Push code to <code>main</code> branch</li>
    <li>GitHub Actions triggers and:
      <ul>
        <li>SSH into EC2</li>
        <li>Pulls the latest code</li>
        <li>Installs dependencies</li>
        <li>Restarts the app using PM2</li>
      </ul>
    </li>
    <li>App is available at <code>http://&lt;EC2-IP&gt;:5000</code></li>
  </ol>

  <h2>📸 Project Screenshots</h2>
  <img src="https://github.com/Birarvindersingh/flask-cicd-app/blob/main/1.PNG" alt="Screenshot 1" width="500" />
  <img src="https://github.com/Birarvindersingh/flask-cicd-app/blob/main/2.PNG" alt="Screenshot 2" width="500" />
  <img src="https://github.com/Birarvindersingh/flask-cicd-app/blob/main/3.PNG" alt="Screenshot 3" width="500" />
  <img src="https://github.com/Birarvindersingh/flask-cicd-app/blob/main/4.PNG" alt="Screenshot 4" width="500" />
  <img src="https://github.com/Birarvindersingh/flask-cicd-app/blob/main/5.PNG" alt="Screenshot 5" width="500" />
  <img src="https://github.com/Birarvindersingh/flask-cicd-app/blob/main/6.PNG" alt="Screenshot 6" width="500" />

  <h2>✅ Conclusion</h2>
  <p>This project helped me understand how to build a basic yet powerful CI/CD pipeline using GitHub Actions and deploy applications to AWS EC2 with secure SSH and PM2. It's a great starting point for cloud-based DevOps practices.</p>

</body>
</html>
