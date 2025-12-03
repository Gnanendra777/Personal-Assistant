# AIVANA

## Main Motive

AIVANA is an intelligent, web-based conversational AI chatbot designed to assist users with both general questions and coding-related tasks. The primary goal is to provide a seamless and persistent chat experience where users can have multiple conversations, which are saved and can be revisited later.

## How It Works

The application provides a chat interface with two distinct modes:

1.  **General Mode**: For conversational, knowledge-based questions and answers.
2.  **Coding Mode**: Specifically tailored to provide code snippets and explanations for programming-related queries.

User conversations are automatically saved to a Firestore database, allowing authenticated users to access their chat history from the sidebar, resume previous conversations, or delete them. The AI responses are generated using Genkit, which connects to the Google Gemini model.

## Features

*   **Dual-Mode AI Chat**: Switch between "General" and "Coding" assistant modes.
*   **User Authentication**: Secure sign-up and login functionality.
*   **Persistent Chat History**: Conversations are saved and linked to the user's account.
*   **Conversation Management**: View, select, and delete past chats from a collapsible sidebar.
*   **Message Editing**: Users can edit their prompts, and the AI will generate a new response.
*   **Theme Toggle**: Switch between light and dark mode for user comfort.
*   **Responsive Design**: A clean and functional UI that works on both desktop and mobile devices.

## Tech Stack

*   **Framework**: Next.js (App Router)
*   **Language**: TypeScript
*   **Styling**: Tailwind CSS
*   **UI Components**: ShadCN UI
*   **Backend & Database**: Firebase (Authentication, Firestore)
*   **Generative AI**: Genkit with Google Gemini

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You will need to have Node.js and npm installed on your machine.

### Installation & Setup

1.  **Clone the repository and install dependencies:**
    ```bash
    git clone <your-repository-url>
    cd <project-directory>
    npm install
    ```

2.  **Set up Environment Variables:**
    Create a new file named `.env.local` in the root of your project and add your Gemini API key:
    ```
    GEMINI_API_KEY=YOUR_API_KEY_HERE
    ```

### Running the Application

1.  **Start the development server:**
    This command runs the Next.js application in development mode.
    ```bash
    npm run dev
    ```

2.  **Open the application:**
    Open your browser and navigate to `http://localhost:9002` (or the port specified in your terminal) to see the application running.