## Transit Morocco App

This is a mobile application for the management of public transport in Morocco. It is a project of the 2end year of the cycle of dvelopment of mobile applications at Youcode Safi , MOROCCO.




## How to install react native expo 
```
npm install -g expo-cli 
```
```
expo init your app 
```
```
expo start
```
or 
```
npx create-expo-app your app 
```
```
npm run web
```
## How to install  react native onboarding swiper
```
npm i react-native-onboarding-swiper
```

# Testing with Jest

```
npx expo install jest-expo jest
```

Then, update package.json to include:

```	
"scripts": {
  ...
  "test": "jest"
},
"jest": {
  "preset": "jest-expo"
}

```
and run render with your version of  react  in this case 18.1.0

```
npm i react-test-renderer@18.1.0
```
-Configuration
A starting configuration you can use is to make sure any modules you are using within the node_modules directory are transpiled when running Jest. This can be done by including the transformIgnorePatterns property that takes a regex pattern as its value:
    
    ```
    "jest": {
      "preset": "jest-expo",
      "transformIgnorePatterns": [
        "node_modules/(?!(jest-)?react-native|react-clone-referenced-element|expo(nent)?|@expo(nent)?/.*|@unimodules/.*|unimodules|sentry-expo|native-base)"
      ]
    }
    ```

for more information about testing with jest [click here](https://docs.expo.io/guides/testing-with-jest/)


# Create Doker image for server

create a Dockerfile in the root of the project
create a .dockerignore file in the root of the project

for build the image
```
docker build -t nameOfyourImage .
```
for run the image
```
docker run -p 5000:5000 -it   nameOfyourImage
```


 