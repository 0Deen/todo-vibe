[![Stand With Palestine](https://raw.githubusercontent.com/TheBSD/StandWithPalestine/main/banner-no-action.svg)](https://thebsd.github.io/StandWithPalestine)

#  <img src="https://github.com/takitajwar17/Simple-Todo-List-Refactored/assets/111155827/4b1c2e01-f24b-4f39-899e-c356d468e386" width="300">

## Simple Todo List App Docs

## Table of Contents

1. [Introduction](#1-introduction)
2. [Project Overview](#2-project-overview)
3. [Getting Started](#3-getting-started)
4. [Code Structure](#4-code-structure)
5. [Dependencies](#5-dependencies)
6. [Code Refactoring](#6-code-refactoring)
7. [Deployment](#7-deployment)
8. [Usage](#8-usage)
9. [License](#9-license)

## 1. Introduction

Welcome to the documentation for the TO-DOIT App, a simple and refactored project designed to manage your tasks efficiently. This document provides an overview of the project, its code structure, refactoring details, clean code practices, design patterns, deployment information, and usage instructions.

## 2. Project Overview

The TO-DOIT App is a web-based application developed to help users manage their tasks by providing a user-friendly interface for adding, editing, and deleting tasks. The app also supports task filtering based on status (All, Pending, Completed) and incorporates a theme switcher for a personalized user experience.

## 3. Getting Started

To get started with the TO-DOIT App, follow these steps:

### Prerequisites

Make sure you have the following installed:

- A modern web browser (e.g., Chrome, Firefox, Safari)
- An internet connection (for fetching external dependencies)

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/0Deen/todo-vibe.git
   ```

2. **Navigate to the Project Directory:**

   ```bash
   cd todo-vibe
   ```

3. **Open `index.html` in a Browser:**

   Open the `index.html` file in your preferred web browser.


## 4. Code Structure

The project follows a modular and organized structure to enhance readability, maintainability, and scalability. Key components include:

- **HTML (`index.html`):** The main structure of the web page.
- **CSS (`style.css`):** Styles to define the appearance of the web page.
- **JavaScript (`main.js`):** Logic for handling user interactions, managing tasks, and implementing theme switching.
- **Fonts (`Poppins`):** Imported from Google Fonts for consistent typography.

## 5. Dependencies

- **Tailwind CSS:** Used for styling the components. It's linked through CDN in the `index.html` file.
- **Daisy UI:** A CSS library for UI components, linked through CDN.
- **Boxicons:** Icons library, linked through CDN.
- **Google Fonts (Poppins):** Font used for the app, linked in the `style.css` file.

## 6. Code Refactoring

### Code Smells Addressed:

1. **Monolithic Structure:**
   - **Code Smell:** Original code had a monolithic structure, making it harder to maintain.
   - **Refactoring:** Introduced modularization through separate classes (`TodoItemFormatter`, `TodoManager`, `UIManager`, and `ThemeSwitcher`), each with a distinct responsibility.

2. **Global Functions:**
   - **Code Smell:** Original code used global functions for event handling, reducing modularity.
   - **Refactoring:** Event handling encapsulated within the `UIManager` class, promoting better organization and separation of concerns.
