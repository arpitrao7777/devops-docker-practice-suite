FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build
WORKDIR /development
COPY . .
RUN dotnet restore
RUN dotnet build --configuration Release
RUN dotnet publish -c Release -o ./publish

FROM mcr.microsoft.com/dotnet/runtime:8.0
WORKDIR /dotnet_artifacts
COPY --from=build /development/publish .
ENTRYPOINT dotnet ElearnBackend.dll