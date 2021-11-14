# Cognito

* The Amplify CLI helps you to create and configure the auth category with an authentication provider.

## Configure Auth Category

* To start provisioning auth resources in the backend, go to your project directory and execute the command:

```
    amplify add auth
```

* Enter the following when prompted:

```
    ? Do you want to use the default authentication and security configuration?
        `Default configuration`
    ? How do you want users to be able to sign in?
        `Username`
    ? Do you want to configure advanced settings?
        `No, I am done.`
```

* To push your changes to the cloud, execute the command:

```
    amplify push
```

## Install Amplify Libraries

* Add the following dependency to your app's build.gradle along with others you added above in Prerequisites and click "Sync Now" when prompted:

```
    dependencies {
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
}
```

## Initialize Amplify Auth

* Add the Auth plugin before calling Amplify.configure
* Check the current auth session