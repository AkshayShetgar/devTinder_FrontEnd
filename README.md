# DevTinder

ssh -i "Tinder-secret.pem" ubuntu@ec2-13-53-41-90.eu-north-1.compute.amazonaws.com
sudo apt update
sudo apt install nginx
sudo systemctl start nginx
sudo scp -r dist/* /var/www/html/
