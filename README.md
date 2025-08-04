# CodeSync

CodeSync is a real-time collaborative coding and video conferencing platform designed for technical interviews. It provides a seamless experience for both interviewers and candidates, enabling them to communicate effectively and work together on coding challenges.

![CodeSync Screenshot](/public/screenshot-for-readme.png)

## Key Features

- **Real-time Video/Audio Interviews:** High-quality video and audio communication powered by Stream.
- **Collaborative Code Editor:** A feature-rich code editor using Monaco Editor that allows multiple users to code simultaneously.
- **Interview Scheduling:** Easily schedule and manage upcoming interviews.
- **Interview Recording:** Record interview sessions for later review.
- **Commenting and Rating:** Interviewers can leave feedback and ratings for each interview.
- **User Roles:** Distinct roles for "interviewer" and "candidate" with different permissions and views.
- **Dashboard:** A centralized dashboard to view upcoming and past interviews.

## Tech Stack

- **Framework:** [Next.js](https://nextjs.org/)
- **Backend & Real-time Database:** [Convex](https://www.convex.dev/)
- **Authentication:** [Clerk](https://clerk.com/)
- **Video & Audio:** [Stream](https://getstream.io/)
- **Code Editor:** [Monaco Editor](https://microsoft.github.io/monaco-editor/)
- **UI:** [Shadcn UI](https://ui.shadcn.com/), [Radix UI](https://www.radix-ui.com/), [Tailwind CSS](https://tailwindcss.com/)
- **Language:** [TypeScript](https://www.typescriptlang.org/)

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- [Node.js](https://nodejs.org/) (version 18 or later)
- [npm](https://www.npmjs.com/)

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/codesync.git
    cd codesync
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    ```

3.  **Set up environment variables:**

    Create a `.env.local` file in the root of your project and add the following environment variables. You will need to get these credentials from the respective services.

    ```env
    # Clerk
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_WEBHOOK_SECRET=

    # Convex
    NEXT_PUBLIC_CONVEX_URL=

    # Stream
    NEXT_PUBLIC_STREAM_API_KEY=
    STREAM_SECRET_KEY=
    ```

4.  **Set up the Convex backend:**

    You will also need to set up the Convex backend. Follow the [Convex documentation](https://docs.convex.dev/getting-started) to get started.

    ```bash
    npx convex dev
    ```

5.  **Run the development server:**

    ```bash
    npm run dev
    ```

    Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Project Structure

-   `convex/`: Contains all the backend logic, including the database schema, queries, and mutations.
-   `src/`: Contains the Next.js frontend application, including pages, components, and hooks.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request
