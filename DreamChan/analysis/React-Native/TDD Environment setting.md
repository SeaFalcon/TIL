# React-Native 환경설정

[TDD 개발 방법론을 활용한 React Native 앱 개발](https://www.inflearn.com/course/React-TDD) 참고

but, 강의 출시일이 1년 6개월전이라서 현 시점에서 RN 환경을 세팅하는것과 좀 달라서 시행착오를 겪음.

## 강의의 TDD 스택 
### Jest + Enzyme + Detox
###### 1. react-native 설치
강의에서는 expo가 아닌 react-native-cli를 사용한다.
Node가 설치되어있다고 가정하고 설치 순서대로 커맨드를 나열하였다.

글로벌로 react-native-cli를 설치하도록 하는데,
공식 사이트에 따르면 글로벌 설치를 추천하지 않는다고 한다.
> If you previously installed a global react-native-cli package, please remove it as it may cause unexpected issues.

따라서 npx 명령어로 react-native를 실행한다.

```sh
# watchman를 설치해야함
brew install watchman 

mkdir rn-practice
cd rn-practice
npx react-native init RNTDD

# 맥북이라 simulator를 사용할 수 있으므로 해당 명령어를 사용해서 실행했다.
npx react-native run-ios
```

위 과정은 [Setting up the development environment](https://reactnative.dev/docs/environment-setup)에서 확인할 수 있다.

###### 2. enzyme 설치

Jest는 자동으로 설치되어있다.
