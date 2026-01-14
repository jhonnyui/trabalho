{
  "name": "frigorifico-vencedor-app",
  "version": "1.0.0",
  "main": "node_modules/expo/AppEntry.js",
  "scripts": {
    "start": "expo start",
    "android": "expo start --android",
    "ios": "expo start --ios",
    "web": "expo start --web",
    "test": "jest",
    "test:watch": "jest --watch",
    "test:coverage": "jest --coverage",
    "lint": "eslint src/**/*.js",
    "build:android": "expo build:android",
    "build:ios": "expo build:ios",
    "publish": "expo publish"
  },
  "dependencies": {
    "@react-native-async-storage/async-storage": "1.21.0",
    "@react-native-community/netinfo": "9.4.1",
    "@react-navigation/bottom-tabs": "^6.5.8",
    "@react-navigation/native": "^6.1.7",
    "@react-navigation/stack": "^6.3.17",
    "expo": "~49.0.15",
    "expo-linking": "~4.0.1",
    "expo-status-bar": "~1.6.0",
    "firebase": "^10.5.0",
    "react": "18.2.0",
    "react-native": "0.72.6",
    "react-native-gesture-handler": "~2.12.0",
    "react-native-maps": "1.7.1",
    "react-native-safe-area-context": "4.6.3",
    "react-native-screens": "~3.22.0",
    "react-native-vector-icons": "^10.0.0",
    "react-redux": "^8.1.3"
  },
  "devDependencies": {
    "@babel/core": "^7.20.0",
    "@testing-library/jest-native": "^5.4.3",
    "@testing-library/react-native": "^12.4.0",
    "babel-jest": "^29.6.4",
    "eslint": "^8.51.0",
    "jest": "^29.6.4",
    "jest-expo": "~49.0.0",
    "react-test-renderer": "18.2.0"
  },
  "jest": {
    "preset": "jest-expo",
    "transformIgnorePatterns": [
      "node_modules/(?!((jest-)?react-native|@react-native(-community)?)|expo(nent)?|@expo(nent)?/.*|@expo-google-fonts/.*|react-navigation|@react-navigation/.*|@unimodules/.*|unimodules|sentry-expo|native-base|react-native-svg)"
    ],
    "setupFilesAfterEnv": [
      "@testing-library/jest-native/extend-expect"
    ],
    "collectCoverageFrom": [
      "src/**/*.{js,jsx}",
      "!src/**/*.test.{js,jsx}",
      "!src/**/__tests__/**"
    ],
    "coverageThreshold": {
      "global": {
        "branches": 80,
        "functions": 80,
        "lines": 80,
        "statements": 80
      }
    }
  },
  "private": true
}
