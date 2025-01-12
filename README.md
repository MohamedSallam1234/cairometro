<p align="center">
<img src="https://cairometro.baraa.app/assets/logo.png" alt="Cairo Metro Logo">
</p>

<h1 align="center">
Cairo Metro
</h1>

An extensive rapid transit system serving the city of Cairo Egypt. The project aims to provide an efficient and
user-friendly application for managing and accessing information about the Cairo Metro.

This project is part of the Software Engineering course at the German International University under the supervision
of [Dr. Amr Desouky](https://github.com/desoukya) and Eng. Ayman Iskandar.

# Screenshots

Click on the images to expand.

<a href="https://github.com/skittlesaur/cairometro/assets/61744498/e1ed3920-73b0-4830-ae00-3f7ecfad2b67" style="display: inline-block; overflow: hidden">
  <img src="https://github.com/skittlesaur/cairometro/assets/61744498/e1ed3920-73b0-4830-ae00-3f7ecfad2b67" alt="Landing Page" style="height: 500px; object-fit: cover; object-position: top;">
</a>

<a href="https://github.com/skittlesaur/cairometro/assets/61744498/20ce5728-bd99-4df2-a747-0386a30e1070" style="display: inline-block; overflow: hidden">
  <img src="https://github.com/skittlesaur/cairometro/assets/61744498/20ce5728-bd99-4df2-a747-0386a30e1070" alt="Subscriptions Page" style="height: 500px; object-fit: cover; object-position: top;">
</a>

<a href="https://github.com/skittlesaur/cairometro/assets/61744498/c4ad1045-7ff9-4dde-a91c-cd66e773970f" style="display: inline-block; overflow: hidden">
  <img src="https://github.com/skittlesaur/cairometro/assets/61744498/c4ad1045-7ff9-4dde-a91c-cd66e773970f" alt="Help Page Example" style="height: 500px; object-fit: cover; object-position: top;">
</a>


<a href="https://github.com/skittlesaur/cairometro/assets/61744498/8ec51bbf-f058-4feb-8b2a-4e17dfd8b07f" style="display: inline-block; overflow: hidden">
  <img src="https://github.com/skittlesaur/cairometro/assets/61744498/8ec51bbf-f058-4feb-8b2a-4e17dfd8b07f" alt="Ticket Details" style="height: 500px; object-fit: cover; object-position: top;">
</a>

<a href="https://github.com/skittlesaur/cairometro/assets/61744498/d316f95e-8024-4556-974d-80047154335c" style="display: inline-block; overflow: hidden">
  <img src="https://github.com/skittlesaur/cairometro/assets/61744498/d316f95e-8024-4556-974d-80047154335c" alt="Login Page" style="height: 500px; object-fit: cover; object-position: top;">
</a>

<a href="https://github.com/skittlesaur/cairometro/assets/61744498/3bc2b4d9-8c41-4d61-86e7-1bb3f2bd4ed4" style="display: inline-block; overflow: hidden">
  <img src="https://github.com/skittlesaur/cairometro/assets/61744498/3bc2b4d9-8c41-4d61-86e7-1bb3f2bd4ed4" alt="Admin Panel" style="height: 500px; object-fit: cover; object-position: top;">
</a>


# Tools & Technologies

- [Linear](https://linear.app): for project management
- [Figma](https://figma.com): for UI/UX design
- [Next.js](https://nextjs.org): for the frontend
- [Node.js](https://nodejs.org): for the backend
- [MongoDB](https://mongodb.com): for the database

# Features

- **Station Information**:
  Provides detailed information about each station, including its location, lines it serves, and nearby landmarks.
- **Route Planning**:
  Allows users to plan their trips by selecting their starting and ending stations, and the app will provide them with
  the best route to take.
- **Ticketing System**:
  Facilitates the purchase and management of tickets, including options for single rides, daily passes, and monthly
  subscriptions.
- **User Profiles**:
  Allows users to create accounts and manage their information, including their tickets and payment methods.
- **Admin Dashboard**:
  Provides an interface for admins to manage the system, including adding new stations, managing tickets, and viewing
  statistics.
- **Customer Support**:
  Provides a way for users to contact customer support and report any issues they face with a real-time chat system.

# Installation and Usage

To run the project locally, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/skittlesaur/cairometro.git
```

2. Install the dependencies:

```bash
cd cairometro
yarn install
```

3. Set up the environment variables:

```bash
cp .env.example .env
```

Then, fill in the required variables in the `.env` file.

4. Run the development server:

```bash
yarn dev
```

**Authentication Note**:

The project requires `hosts` file configuration to work properly. Add the following line to your `hosts` file:

```
::1       cairometro
127.0.0.1 cairometro
::1       api.cairometro
127.0.0.1 api.cairometro
```

Run the frontend at [http://cairometro:3000](http://cairometro:3000) and the backend at [http://api.cairometro:1111](http://api.cairometro:1111).

# Repository Structure

The repository follows the following structure:

```text
├── apps
│   ├── graphql
│   │   ├── prisma   # Prisma schema and nexus types
│   │   └── src
│   │       ├── api  # Public Express API
│   │       ├── lib  # Utility functions
│   │       ├── notifications  # Notification templates in mjml
│   │       ├── permissions  # Permissions for the GraphQL API
│   │       ├── resolvers    # GraphQL resolvers
│   │       │   ├── mutations
│   │       │   └── queries
│   │       ├── types        # GraphQL types
│   │       └── utils        # Utility functions
│   └── home
│       ├── components  # React components
│       ├── context     # React context
│       ├── graphql     # GraphQL queries and mutations
│       ├── help        # Help pages markdown files
│       ├── icons       # SVG icons
│       ├── layouts     # React layouts
│       ├── lib         # Utility functions
│       ├── pages       # Next.js pages
│       ├── public      # Public assets
│       ├── styles      # CSS styles
│       └── types       # TypeScript types
```