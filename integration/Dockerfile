FROM microsoft/dotnet:2-sdk
WORKDIR /integration

COPY integration.csproj .
RUN dotnet restore
ENV TEAMCITY_PROJECT_NAME=fake
COPY . .
ENTRYPOINT ["dotnet", "test"]