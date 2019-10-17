
# Add vagrant user to docker group
sudo groupadd docker
sudo usermod -aG docker vagrant
newgrp docker

# Run Docker at startup
sudo systemctl enable docker
