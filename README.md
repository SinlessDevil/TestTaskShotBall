🎮 Shot Ball — Test Task Alta Games
<p align="center"> <a href="https://www.youtube.com/watch?v=tkuuGagN_kM&t=13s" target="_blank"> <img src="https://img.youtube.com/vi/tkuuGagN_kM/0.jpg" alt="Watch the demo" /> </a> </p> <p align="center"> <a href="https://www.youtube.com/watch?v=tkuuGagN_kM&t=13s" target="_blank"> <img src="https://img.shields.io/badge/Watch%20on-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube" /> </a> </p>

Gameplay : On the screen is the balloon player in the lower left corner, and the target in the upper right corner, where the ball must hit. The path is blocked by obstacles. The ball player creates shots due to its size, it is necessary to clear a path for the ball player to jump along the cleared path to the final goal.

---
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/main/Screenshot/GamePlay_Shot_Ball_1.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/main/Screenshot/GamePlay_Shot_Ball_2.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/main/Screenshot/GamePlay_Shot_Ball_3.png)
# Game logic
>Button through action

I made all the buttons on the stage through Action. It's quite convenient to subscribe to buttons + buttons don't know what they are responsible for, and this is its main advantage. This script generally complies with the SRP principle, so it can be used in other projects.
I also implemented a simple State machine. Where I switch panels.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Button_AddListener_1.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Button_AddListener_2.png)

---
>Patten Singletone

Implemented the Singletone pattern for Audio Managera, Pool Mono, Save System.
Singleton is a creational design pattern, which ensures that only one object of its kind exists and provides a single point of access to it for any other code.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Pattern_Singletone.png)

---
>Patten Observer

Interaction of interfaces and the GamePlay itself has always done with the help of Action.
Observer is a behavioral design pattern that allows some objects to notify other objects about changes in their state.
The Observer pattern provides a way to subscribe and unsubscribe to and from these events for any object that implements a subscriber interface.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Pattern_Observer.png)

---
>Pattern Pool Objects

For the effects that I play after each destruction of objects, I decided to use Pool Object to save memory.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Pattern_PoolMono.png)

---
>Pattern Factory

For bullets still decided to make a regular factory, for the reason that they are not as often call as effects, but you can still think about pool objects.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Pattern_Factory.png)

---
>Shot System

Made this module, the basis of this Shot can be said to be the access point to this module. Shot Reload - reload the weapon, Shot SizeTransfer - pumps the size of the ball into the bullet. Push Bullet - the bullet itself. (I also separated the logic here, on the bullet factory, and the Shot Direction itself.)

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Shot_System_4.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Shot_System_1.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Shot_System_2.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Shot_System_3.png)

---
>OOP

Wherever there were more than two implementations, I made a hierarchy of inheritance through abstraction.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/OOP.png)

---
>Aniamtion Player Jump - Open Door

I made an animation for the player when jumping using the "box in the butt" method. This is when the box is attached to the character to his center with Joint.
Also the door is also made through the joint.

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Box_Ass.png)
![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/HingeJoin.png)

---
#FrameWork
---
>UnitRx

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/FrameWork_UniRx.png)

>Zenject

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/FrameWork_Zenject.png)

>DoTween

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/FrameWork_DoTween.png)

---
#Extensions
---
>Button Extensions

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Extentions_Button.png)

>Transform Extensions

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Extentions_Transform.png)

>LogError Extensions

![Image alt](https://github.com/SinlessDevil/Test_Task_Shot_Ball/blob/Fixed/Screenshot/Extentions_Transform.png)

---
For now, that's it. =)
