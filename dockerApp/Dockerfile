#Depending on the operating system of the host machines(s) that will build or run the containers, the image specified in the FROM statement may need to be changed.
#For more information, please see http://aka.ms/containercompat 

FROM microsoft/aspnet:4.7.2-windowsservercore-1803
ARG source
SHELL ["powershell"]
EXPOSE 80
WORKDIR /inetpub/wwwroot
COPY ["https://github.com/charankumar4321/dockerApp.git":c:\wwwrot\intpub]
CMD ["dockerapp","-DFOREGROUND"]
ENTRYPOINT ["dotnet", "dockerApp.dll"]
