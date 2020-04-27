## React Redux Notes

### EN
Coming soon.

### TR

## Redux Nedir ?
*Geliştirici: Dan Abramov
*Kütüphane'dir.
*State'leri yönetmeyi sağlar.
*Application State Management
*state geçmişini tutabilir.

## Kurulum: 
npm install redux react-redux --save

Store Oluşturma;

index.js içinde;

import {createStore} from "redux";

const store = createStore();

## Store'u Component'e bağlama işlemi;

App.js içinde;

import {connect} from 'react-redux'

export default connect()(App);



## Redux Veri Akışı
**Dispatcher etmek ; Action'da ki data'yı store'a göndermek demektir.** <br>
**View > Actions > Store(Dispatcher > Reducer > State) > View** <br>
**Reducer'lar Store tarafından veriyi alır istenildiği gibi günceller store'a tekrardan göndermiş olur.** <br>
**Store Subscribe metodu: Action Dispatch olduğunda  değişiklik olduğunda çalışır.** <br>
**combineReducer: Birden fazla reducerler için birleştirme gerekli bunu combineReducer ile yapıyoruz.** <br>
**Provider: Redux Store un REact uygulamasında erişilebilir olması için provider'ı index.js içinde <Provider store={store}><App /></Provider> olarak sarmalamamız gerekli.** <br> 
**Connect: Store'u COmponentimize bağlamak için kullanıyoruz.** <br>
**mapStateToProps: state içinde ki bilgileri props olarak kullanmamıza yarayan bir mapleme sistemi.** <br>

**Dizin yapısı:** <br> 
src altına yeni klasör > reducers > yeni js dosyası nameReducer.js
src altına yeni klasör > actions > yeni js dosyası name-actions.js


**Redux Thunk**
Kurulum: npm install react-thunk --save
Redux thunk middleware yapısı action yerine fonksiyon dönebilmenizi sağlar.

thunk'ta action yerine fonksiyon dönmemizin tek amacı middleware'e bir nevi sinyal göndermek.

**compose : Birleştirmek iç içe geçirmek.** <br>

**mapDispatchToProps**
Action dispatch etmek için kullanılır.

**mergeProps**
Tüm propsların nereden geldiğini görmek için kullanılır.




## Available Scripts
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
# mehmetdilmen03-gmail.com
