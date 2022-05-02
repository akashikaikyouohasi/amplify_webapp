# 概要

AWSのチュートリアルの「React アプリケーションの構築 AWS Amplify を使用してシンプルなウェブアプリケーションを作成する」を行うためのリポジトリです。

## 実行手順
### 初期化
```
npx create-react-app amplify-web-app
cd amplify-web-app/
npm start
cd ../
git init
git remote add origin git@github.com:akashikaikyouohasi/amplify_webapp.git
git add .
git commit -m "initial commit"
git push origin master
vim src/App.js
git add .
git commit -m "change for v2"
git push origin master
```

### Amplify CLI
#### インストール
```
npm install -g @aws-amplify/cli
```

#### 設定
```
amplify configure
# amplify init --appId [your-app-id]
例：amplify init --appId d3d3neebmk8ys5
```

#### Amplifyライブラリインストール
```
npm install aws-amplify @aws-amplify/ui-react
```

#### 認証サービスの追加
```
# amplify add auth
Using service: Cognito, provided by: awscloudformation
 
 The current configured provider is Amazon Cognito. 
 
 Do you want to use the default authentication and security configuration? Default configuration
 Warning: you will not be able to edit these selections. 
 How do you want users to be able to sign in? Username
 Do you want to configure advanced settings? No, I am done.
✅ Successfully added auth resource amplifywebappc2363d24 locally

✅ Some next steps:
"amplify push" will build all your local backend resources and provision it in the cloud
"amplify publish" will build all your local backend and frontend resources (if you have hosting category added) and provision it in the cloud
```

