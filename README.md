# FaalGUI Application

## Overview

FaalGUI is a Java Swing-based GUI application that fetches and displays a random Persian poem (Faale Hafez) and its interpretation from an online API. The user can generate a new poem by clicking a button and navigate between the home page and the poem display page.

## Features

- Fetches random Persian poems and interpretations from an online API.
- Displays the fetched poem and interpretation in a user-friendly GUI.
- Uses Persian font(Nazanin) for a better user experience.

## Requirements

- Java 8 or higher
- jackson-core library (link: <https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-core/2.17.1>)
- jackson-annotations library (link: <https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-annotations/2.17.1>)
- jackson-databind library (link:<https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-databind/2.17.1>)
(or you can add maven to your project and add the dependency below to pome.xml:
- `com.fasterxml.jackson.core:jackson-databind:2.13.3`
)

## Usage

- **Home Page**: The home page displays a prompt for the user to make a wish and click the button to get a Faal.
- ![Main Menu](https://github.com/Kosar-Gari/FaaleHafez/blob/main/Screenshots/HomePage%20Panel.png)
The background color of the home page is set to Shirazi color (RGB: 178, 9, 49)
- **Get Faal Button**: Clicking the "دریافت فال" (Get Faal) button fetches a random poem and its interpretation from the API and navigates to the Poem Page.


- **Poem Page**: After clicking the button, the application fetches a poem and its interpretation from the API and displays it.
- ![Main Menu](https://github.com/Kosar-Gari/FaaleHafez/blob/main/Screenshots/Poem%20%26%20Interpretation%20Panel.png)
- **Back Button**: Use the back button to return to the home page.

## Code Explanation

### Main Components

- **FaalGUI Class**: The main GUI class that handles the UI components and interactions.
- **Faal Class**: A simple data class to hold the poem and interpretation.

### Methods

- **getFaal()**: Fetches a random poem and interpretation from the API.
- **HomePage()**: Sets up the home page UI components.
- **FaalPage(String poem, String interpretation)**: Sets up the poem display page UI components.
- **actionPerformed(ActionEvent e)**: Handles button click events to switch between pages.

### Customizations

- **Font and Colors**: Custom Persian fonts and colors are used to enhance the user interface.
