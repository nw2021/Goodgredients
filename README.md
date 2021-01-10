![Image of Logo](https://raw.githubusercontent.com/nw2021/Goodgredients/main/img/logo/KakaoTalk_Photo_2021-01-09-22-32-26.png)

Have you ever wondered what's actually in your shampoo or body wash?
Have you ever been concerned about the toxicity of certain chemicals in them on your body and to the environment?

If you answered *yes*, you came to the right place. 
Welcome to the wonderful world of Goodgredients! 😀

Goodgredients provides a simple way to answer these questions.
But *how* you may ask.

The core of this application is Salesforce Einstein Vision. In particular, we are using Einstein OCR (Optical Character Recognition), which uses deep learning models to detect alphanumeric text in an image. [You can find out more info about Einstein Vision here.](https://metamind.readme.io/docs/what-is-the-predictive-vision-service)

Essentially, we've created a [backend api service](https://github.com/nw2021/GoodgredientsBack) that takes an image request from a client, uses the Einstein OCR model to extract text from the image, compares it to our dataset of chemical details (ex. toxicity, allergy, etc.), and sends a response containing the comparison results back to the client.

To demonstrate a practical workflow, we've also created a [sample client iOS app using React Native.](https://github.com/nw2021/GoodgredientsFront)

## demo
![demo gif](img/goodgredientsdemo.gif)
