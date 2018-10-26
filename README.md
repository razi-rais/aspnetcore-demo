# aspnetcore-demo
Simple demo showing cross platform features of asp.net core 

Before you begin make sure to clone the repo and land in the correct directory. 

git clone https://github.com/razi-rais/aspnetcore-demo.git 
cd aspnetcore-demo


# Build & Run Instructions for Mac OS & Linux

On mac OS and Linux Ubuntu 16.04 you need to install following software 

### Prerequisites 
* .NET Core 2.1.403 SDK (https://www.microsoft.com/net/download)
* Docker - mac OS (https://www.docker.com/products/docker-desktop) | Linux (https://www.docker.com/products/docker-engine)

## Building the application

dotnet build 

## Run the application locally

dotnet run 

## Test the application 

Open browser and navigate to the URL: http://localhost:5000. You should see a basic web page with top menu pointing to various sections of the website. Close the browser and make sure you stop the dotnet application runtime by going back to terminal and pressing CTRL + C key combination. You want to make sure that port 5000 is now available.

# Building Docker Image 

docker build -t aspnetcore-demo:dev -f Dockerfile.Linux .

# Running the Docker Container

docker run -p 5000:5000  aspnetcore-demo:dev  

## Test the application runnin inside the container 

Open browser and navigate to the URL: http://localhost:5000. You should see a basic web page with top menu pointing to various sections of the website.






