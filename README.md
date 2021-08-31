# CATastrophe

- This project is a study app that motivates you to focus or else there will be a catastrophe! (pun intended)

- The user sets a timer of X minutes and after the timer has finished, you're rewarded with a cat picture that is stored in your previous tasks to view.

     - Failure to complete the timer will result in a deduction of coin balances in the shop where you can buy other animals and get rewarded with their pictures

## Usage

- The project is currently in the MVP stage and will be released in the near future publicly on the Google Playstore and Expo!

## Tech Stack

### Client

- The client is a TypeScript + React Native Expo application styled with UI Kitten Components hosted as unlisted on Expo.

- AsyncStorage is used to store the logged in user's JWT token coming from the Apollo GraphQL Client's requests to the GraphQL API.

- Routing is handled with React Router Native along with theming coming from Eva's design system.

### Server

- The server is a TypeScript + Node Apollo GraphQL server hosted on an Amazon EC2 instance and MySQL RDS Database Instance.

- Prisma acts as the ORM to fetch task and user data along with jsonwebtoken generating jwts to authenticate and authorize user requests

- Passwords are hashed with bcrypt and authentication is handled with JWT's while requests are tested with Jest

## Future Plans

- ⬜️ Allow users to organize their completed tasks by tag and update/delete tasks if needed

- ⬜️ Implement boosts and rewards to receive more pictures after a task has been completed/multiple tasks have been completed (more coins rewarded as a multiplier)

- ⬜️ Integrate OAuth Authentication with major providers like Google and Github
