# Madrasty

## Overview

Madrasty is a comprehensive software solution designed to streamline and automate various administrative and operational processes within a school. The system aims to improve efficiency and provide better tracking and reporting capabilities for the school’s management, teachers, students, and parents.

Despite technological advancements, many schools still rely on paper-based methods for a variety of administrative activities. Even though some schools have made progress toward automation, they often use a combination of paper-based systems and small-scale digital solutions, each designed for a specific task. This approach can lead to inefficiencies, data inconsistencies, and difficulties in accessing timely and accurate information. The lack of integration between these systems results in challenges such as poor administration, data loss, lengthy processes, and limitations in meeting the specific needs of the schools.

Additional issues include:
- **Teachers**: Managing classes and materials, creating activities, and tracking each student's performance.
- **Guardians**: Difficulty in tracking their children’s performance and behavior.

## System Architecture

### Overview
The Madrasty system is designed with a decoupled backend and client-side application setup, utilizing a RESTful API. This architecture supports future integration of various client platforms, as opposed to the traditional Model-View-Controller (MVC) pattern, which is typically tied to web applications.

### Back-end Architecture
We adopted the Clean Architecture principle, which is organized into four primary layers, ensuring a clear separation of concerns and maintainability:
- **Data Layer**: Defines the domain entities crucial for the business logic.
- **Data Access Layer**: Facilitates interactions with data repositories, ensuring data integrity and consistency.
- **Cross-Cutting Layer**: Provides shared services and dependencies that are used across multiple layers.
- **Service Layer**: Implements the core business logic and performs necessary validations.
- **Presentation Layer**: Acts as the interface to our RESTful API, enabling client applications to interact with the backend.

Additionally, we incorporated a Modular Monolith Architecture to cater to specific business requirements, such as the option to offer either the Administrative Module alone or both the Administrative and Engagement Modules together.

### Client-Side Application
For the client-side application, we initiated development with a web application to ensure accessibility across various platforms. We selected the open-source React framework due to its extensive community support and robust ecosystem.

This architectural setup not only meets our current project requirements but also positions us for future scalability and flexibility, allowing for easy integration of additional client platforms and modules as needed.

![Arch](https://github.com/Hadymohammed/About-Madrasty/assets/50783061/ad9dcae7-2e1f-4cea-a498-b54daf5f0eb1)



## Technologies
The system was implemented using:
- **Backend**: C#, ASP .NET CORE, and Entity Framework (ORM)
- **Database**: MS SQL (Relational Database)
- **Frontend**: React, Tailwind CSS, and Yup
- **Deployment**:
  - Azure: To deploy the web API
  - SmarterAsp: For the database
  - Render: For the frontend
- **CI/CD**: GitHub Actions

## Team Members
- [**Abdelhady Mohamed**](https://github.com/Hadymohammed): FullStack Developer and Team Leader
- [**Alyaa Elhawary**](https://github.com/alyaa999): Backend Engineer
- [**Asmaa Khamis**](https://github.com/AsmaaKhamis1911): Backend Engineer, Documentation
- [**Mohamed Omran**](https://github.com/MohamedOmran890): Backend Engineer
- [**Nada Hamdi**](https://github.com/Nada0Hamdi): Product Manager and Backend Engineer
- [**Nada Khaled**](https://github.com/nadaKhalid13): UI/UX Designer and Frontend Engineer
- [**Mohamed Yasser**](https://github.com/Mhmdyasser33): Frontend Engineer
- [**Mahmoud Shaban**](https://github.com/mahmoud-sh3aban): Frontend Engineer

## Demo Result
**Note**: You might experience starting latency due to the free subscription capabilities.

- **API**: [Swagger Documentation](https://madrasty-api.azurewebsites.net/swagger/index.html)
- **Administrative Client App**: [Madrasty Admin](https://madrasty.onrender.com/login)
  - **Username**: Super@madrasty.com
  - **Password**: Super@1234

- **Engagement Client App**: [Madrasty Engagement](https://mardasty-engagement.onrender.com/login)
  - **Username**: Instructor@madrasty.com / Student@madrasty.com / Guardian@madrasty.com
  - **Password**: User@123

- [**Final Presentation.**](https://docs.google.com/file/d/1K1VGwoPnbVUZaQmDyN0I6AAd1HIm5dnf/edit?usp=docslist_api&filetype=mspresentation)
