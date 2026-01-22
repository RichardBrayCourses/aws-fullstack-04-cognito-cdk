# To Run This Application

## 1. Install pnpm libraries

```
pnpm install
```

## 2. Bootstrap the CDK

```
pnpm bootstrap-up
```

Note that there is also a bootstrap-down command to remove the bootstrap: this should only be done if all CloudFormation stacks have been deleted first.

## 3. Deploy cognito

Deploy cognito with the CDK

```
pnpm deploy-cognito
```

## 4. Update cognito values in .env file

Note the cognito domain and client id and update the file ui/.env, replacing the values below:

```
VITE_COGNITO_DOMAIN='https://eu-west-2azp1ieq4o.auth.eu-west-2.amazoncognito.com'
VITE_COGNITO_CLIENT_ID='1ctvlmhfehrj0dumbmb2tv1shp'
```

## 5. Build and Run the UI

```bash
pnpm dev
```

Then follow the browser link.

## 6. Login

Select "Login" and create a new user login ...
