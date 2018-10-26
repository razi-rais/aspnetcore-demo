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

## Building Docker Image 

docker build -t aspnetcore-demo:dev -f Dockerfile.Linux .

## Running the Docker Container

docker run -p 5000:5000  aspnetcore-demo:dev  

## Test the application running inside the container 

Open browser and navigate to the URL: http://localhost:5000. You should see a basic web page with top menu pointing to various sections of the website.


# Build & Run Instructions for Windows Server 2016 

These instructions are tested on Windows Server 2016 (version 1607). I mainly use Windows Server 2016 as it comes with native Windows Container support. You should also able to run .NET core application locally without issues on Windows 10 but building container image is heavily dependent on host operating system version. Don't be surprise if exact image tag used in this document does not work for your version of Windows. 

Here are two articles that go deeper into what I am talking about. Read them carefully or get toasted. 
* https://github.com/dotnet/announcements/issues/38 
* https://docs.microsoft.com/en-us/virtualization/windowscontainers/deploy-containers/version-compatibility

### Prerequisites 
* .NET Core 2.1.403 SDK (https://www.microsoft.com/net/download)
* Docker - mac OS (https://www.docker.com/products/docker-desktop) | Linux (https://www.docker.com/products/docker-engine)

## Building the application




