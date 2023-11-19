# Use the official .NET SDK image for building the application
FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build
WORKDIR /src

# Copy the solution file and restore dependencies
COPY ["Portfolio.sln", "."]
COPY ["src/app/app.csproj", "src/app/"]
COPY ["src/lib/lib.csproj", "src/lib/"]

RUN dotnet restore "src/app/app.csproj"
RUN dotnet restore "src/lib/lib.csproj"

# Copy the entire solution and build the application
COPY . .
WORKDIR "/src/src/app"
RUN dotnet build "app.csproj" -c Release -o /app/build

# Build the application for publishing
FROM build AS publish
RUN dotnet publish "app.csproj" -c Release -o /app/publish

# Use the official .NET runtime image for the final image
FROM mcr.microsoft.com/dotnet/aspnet:8.0 AS final
WORKDIR /app
EXPOSE 80

# Copy the published output from the 'publish' stage
COPY --from=publish /app/publish .

# Set the entry point for the application
ENTRYPOINT ["dotnet", "app.dll"]
