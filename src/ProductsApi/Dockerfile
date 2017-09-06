FROM microsoft/dotnet:latest
RUN apt-get update && apt-get install -y dotnet-sdk-2.0.0

MAINTAINER Julien Corioland, Microsoft (@jcorioland)

WORKDIR /app
ENTRYPOINT ["dotnet", "run"]
EXPOSE 5000

ENV ASPNETCORE_URLS http://+:5000

COPY project.json ./
RUN pwd
RUN dir
RUN ls -lrt


COPY . /app
RUN ["dotnet", "build"]
