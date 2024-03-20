# Djoufson's awesome portfolio ✨

Welcome to the source code repository of my personal portfolio website. This website is built using the brand new Blazor SSR, showcasing my skills, projects, and experiences.

[Visit the site here 🌍](https://djoufson-tech.azurewebsites.net)

![Screenshot](/docs/screenshot.png)

## Table of Contents

- [Introduction](#introduction)
- [License](#license)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Run](#run)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Introduction

This portfolio website serves as a platform to showcase my professional experience, skills, and projects. It is designed to provide a clean and interactive interface for visitors to learn more about me and my work.

## License

This project is licensed under the [MIT License](LICENSE).
Read carefully the License

## Features

- **Responsive Design:** The website is designed to be responsive, ensuring a seamless experience across various devices.
- **Project Showcase:** Highlight your key projects with detailed descriptions and links.
- **Skills Section:** Display your skills in a visually appealing manner.
- **Contact Form:** Allow visitors to get in touch with you easily through a contact form.
- **Interactive Elements:** Leverage Blazor WebAssembly to create dynamic and interactive components.

## Getting Started

### Prerequisites

### **For local development**

- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0) installed
- [Visual Studio](https://visualstudio.microsoft.com/) or [Visual Studio Code](https://code.visualstudio.com/) for development (optional)

### **Inside Docker Container**

- [Docker Desktop](https://docs.docker.com/engine/install/) installed

### Installation

- Clone the repository:

  ``` shell
  git clone https://github.com/Djoufson/Portfolio.git
  ```

- Navigate to the project folder:

  ``` shell
  cd Portfolio
  ```

### Run

### **Locally**

- Restore dependencies:

  ``` bash
  dotnet restore
  ```

- Build the project:

  ``` bash
  dotnet build
  ```

- Run the application:

  ``` bash
  dotnet run --project src/app
  ```

### **Inside Docker Container-**

- Launch the Docker Desktop software and wait for it to start
- Run the application:

  ``` bash
  docker-compose up
  ```

## Usage

Customize the content of the website to reflect your personal and professional information. Update the projects, skills, and experiences in the respective sections.

## Folder Structure

``` md
/portfolio
|-- src/
| |-- app/
| | |-- Components/
| | |-- scss/
| | |-- wwwroot/
| | |-- app.csproj
| | |-- Dockerfile
| | |-- Program.cs
| |-- lib/
| | |-- ...
|-- .dockerignore
|-- .gitignore
|-- docker-compose.yml
|-- package.json
|-- Portfolio.sln
|-- README.md
```

- **src:** Contains the Blazor application and the `lib` project for any external dependencies.

## Technologies Used

- [Blazor SSR](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
- [C#](https://docs.microsoft.com/en-us/dotnet/csharp/)
- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [SCSS](https://sass-lang.com/install/)

## Contributing

If you'd like to contribute, please fork the repository and create a pull request. For major changes, please open an issue first to discuss the proposed changes.

## Acknowledgments

I would like to express my gratitude to the following individuals and resources that have contributed to the development and inspiration of this portfolio website:

- **Open Source Community:** I want to personally thank [Yanka Darelova](https://twitter.com/YankaDarelova) for the amazing free Figma design I used. You can use the same if you want, it is available [here](https://www.figma.com/community/file/1100794861710979147). Give a like ❤️
