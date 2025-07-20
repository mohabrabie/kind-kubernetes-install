# installing kubernetes cluster using Kind on Ubuntu 🚀
in this documentation I will show you the steps of creating a cluster using kind locally and allowing access for a specific IP to the APIServer and run commands on the Master

## Installation 💻

![Screenshot](1.png)
![Screenshot](2.png)
![Screenshot](3.png)
![Screenshot](4.png)
![Screenshot](5.png)
![Screenshot](6.png)
![Screenshot](7.png)
![Screenshot](8.png)

### Prerequisites
- 2 VMs ubuntu 22.04 installed on them
- Docker installed on the server

### Steps
```bash
# Clone the repository
git clone https://github.com/username/project-name.git

# Install dependencies
pip install -r requirements.txt
npm install

# Set up environment variables
cp .env.example .env