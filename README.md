# EFGetStarted

Get Started dotnet ef core 6.0 run on Ubuntu with raspberry pi 4.

#Usefull to have on .bashrc
echo "${PATH//:/$'\n'}"
export PATH=$PATH:/usr/bin/dotnet
export PATH="$PATH:/home/doug/.dotnet/tools"

EF
https://www.nuget.org/packages/dotnet-ef/
dotnet tool install --global dotnet-ef --version 6.0.0
dotnet new tool-manifest # if you are setting up this repo
#Paleative option in order to run db locally
dotnet tool install --local dotnet-ef --version 6.0.0

dotnet ef migrations add InitialCreate