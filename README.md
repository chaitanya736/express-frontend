# express-frontend


# CI/CD Deployment: Flask & Express on EC2

## Overview
This project deploys a Flask backend and Express frontend on a single EC2 instance and automates deployments using Jenkins.

## Tech Stack
- AWS EC2
- Flask
- Express
- Jenkins
- PM2
- GitHub Webhooks

## Access
- Flask: http://<EC2_IP>:5000
- Express: http://<EC2_IP>:3000

## CI/CD Flow
GitHub → Jenkins → EC2 → PM2 Restart
