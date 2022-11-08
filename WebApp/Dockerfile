
FROM mcr.microsoft.com/dotnet/aspnet:6.0
COPY bin/Release/net6.0/publish App/
ADD bin/cert/ /etc/ssl/certs
RUN update-ca-certificates
WORKDIR /App
ENTRYPOINT ["dotnet", "WebApp.dll"]

