# 🚀 Static Website with CI/CD on AWS S3

This project demonstrates how to deploy a static website (HTML/CSS/JS) to **Amazon S3** with **automated CI/CD using GitHub Actions**.

Whenever you push changes to the `main` branch, the site is automatically deployed to your S3 bucket. ✨

---

## 🗂️ Project Structure


├── index.html ├── styles.css ├── .github/ │ └── workflows/ │ └── deploy.yml └── README.md


---

## ⚙️ CI/CD Workflow

The GitHub Actions workflow:

1. Triggers on pushes to `main`
2. Configures AWS credentials securely using GitHub Secrets
3. Syncs the project files to the configured S3 bucket: `my-static-site-arjun`

---

## 🧪 How to Use

### 1. Clone the repo

```bash
git clone https://github.com/arjunnbr97/static-cicd-site.git
cd static-cicd-site

###


2. Set Up GitHub Secrets
Go to your repo settings > Secrets and variables > Actions and add:
Name	Description :

AWS_ACCESS_KEY_ID	    Your AWS access key
AWS_SECRET_ACCESS_KEY	Your AWS secret key
AWS_REGION	          ap-northeast-1
S3_BUCKET           	my-static-site-arjun

###

git add .
git commit -m "Initial commit"
git push origin main

###






