# DevTinder

ssh -i "Tinder-secret.pem" ubuntu@ec2-13-53-41-90.eu-north-1.compute.amazonaws.com
sudo apt update
sudo apt install nginx
sudo systemctl start nginx
sudo scp -r dist/* /var/www/html/



# Backend
install pm2
pm2 logs
pm2 start npm -- start
pm2 stop <name>
pm2 delete <name>
pm2 list
pm2 start npm --name "" start
sudo nano /etc/nginx/site-available/default


nginx config : 
 location /api {
        proxy_pass http://localhost:3000;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }

    sudo systemctl restart nginx





    aws_secret_key = "tF+YTP3wKp2SjS+/RXhOVgyp0tjosONrgb2rHHJx"

    aws_access_key = "AKIAWX2IFLQDBPCTZFUX"

    https://razorpay.me/@akshaykumar2461



    RazorPay Gateway - 
    - install razorPay
    - config instance / order
    - create API for payment gateway
    - you need to create order using create() and option
    - save the data in db
    - call api using axios 



    WebSockets ----- Real time chating(Socket.io)