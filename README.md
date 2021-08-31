# CATastrophe

- This project is a study app that motivates you to focus or else there will be a catastrophe! (pun intended)

- The user sets a timer of X minutes and after the timer has finished, you're rewarded with a cat picture that is stored in your previous tasks to view.

     - Failure to complete the timer will result in a deduction of coin balances in the shop where you can buy other animals and get rewarded with their pictures

## Usage

- The project is currently in the MVP stage and will be released in the near future publicly on the Google Playstore and Expo!

Current Screens (Images are too large for README) : [https://imgur.com/a/6vWeJJY](https://imgur.com/a/6vWeJJY)

## Tech Stack

### Client

- The client is a [TypeScript](https://www.typescriptlang.org/) + [React Native Expo](https://expo.dev/) application styled with [UI Kitten](https://akveo.github.io/react-native-ui-kitten/) Components hosted as unlisted on Expo.

- [AsyncStorage](https://react-native-async-storage.github.io/async-storage/) is used to store the logged in user's [JWT token](https://jwt.io/) coming from the [Apollo GraphQL Client's](https://www.apollographql.com/docs/react) requests to the [GraphQL](https://graphql.org/) API.

- Routing is handled with [React Router Native](https://reactrouter.com/native) along with theming coming from [Eva's design](https://colors.eva.design/) system.

### Server

- The server is a [TypeScript](https://www.typescriptlang.org/) + [Node](https://nodejs.org/en/) [Apollo GraphQL Server](https://www.apollographql.com/docs/apollo-server/) hosted on an AWS [EC2](https://aws.amazon.com/ec2/) instance and [MySQL RDS](https://aws.amazon.com/rds/) Database Instance.

- [Prisma](https://www.prisma.io/) is the ORM to fetch task and user data along with [jsonwebtoken](https://www.npmjs.com/package//jsonwebtoken) generating [JWT's](https://jwt.io/) to authenticate and authorize user requests

- Passwords are hashed with [bcrypt](https://www.npmjs.com/package/bcryptjs) and authentication is handled with [JWT's](https://jwt.io/) while requests are tested with [Jest](https://jestjs.io/)

## Future Plans

- ⬜️ Allow users to organize their completed tasks by tag and update/delete tasks if needed

- ⬜️ Implement boosts and rewards to receive more pictures after a task has been completed/multiple tasks have been completed (more coins rewarded as a multiplier)

- ⬜️ Integrate OAuth Authentication with major providers like Google and Github
