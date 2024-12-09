# Expo Android Intermittent Crashes

This repository demonstrates a bug encountered in an Expo app running on Android. The app crashes intermittently without providing clear error messages in the console. The crashes appear to be linked to asynchronous operations and frequent screen navigation using React Navigation.

## Bug Description

The app crashes sporadically on Android devices.  No specific error messages are displayed, making debugging difficult. The frequency of crashes increases with rapid screen transitions.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `expo start`.
4. Rapidly navigate between screens.  The app might crash after a few transitions.

## Solution

The solution involved carefully reviewing the asynchronous operations and ensuring proper error handling within the navigation process.  Asynchronous tasks were checked for potential race conditions or unhandled rejections.  Implementation of more robust error handling improved stability.