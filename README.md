# 🏠 Gathering Resources — Unreal Engine 5 🎮🛠️

[🎥 YouTube Preview ▶️](https://youtu.be/mRkBQJUswpk)

![Preview Image](https://sun9-80.userapi.com/s/v1/ig2/zGLrUcR_scvf0yXvu2sKw7ykKK31dJQgaC91NL7-f6EuVaBO3-9PiIEazqrm7s-0Srq-NQ3ydzQSL5Gio-bqvBrM.jpg?quality=95&as=32x32,48x48,72x72,108x108,160x160,240x240,360x360,480x480,540x540,640x640,720x720,1024x1024&from=bu&cs=1024x0)

---

## 📖 Implementation in your project | Внедрение в ваш проект

**RU:**
1. Добавьте компонент BPAC_GatheringComponent в место по вашему выбору (персонаж или состояние игрока).
2. Добавьте интерфейс (BPI_GetMesh) к вашему классу персонажей и передайте скелетную сетку, чтобы получить функцию Pawn Mesh. Чтобы добавить интерфейс, вам нужно выбрать ClassSettings и в правой части панели сведений найти вкладку Интерфейсы.  
![Интерфейс](https://sun9-17.userapi.com/s/v1/ig2/_IjaQQQbi6ah3EDxIEJo-udtrnC4QiacD_bUyBGHbAV4qZxx2DwIwnPC4uBJvKx9fGIZCKy9pDUAu3rldeqxOriV.jpg?quality=95&as=32x5,48x7,72x10,108x16,160x23,240x35,360x52,480x69,540x78,581x84&from=bu&cs=581x0)  
3. Добавьте интерфейс (BPI_GetComponents) к классу вашего персонажа и к контроллеру игрока! и передайте GatheringComponent функции GetGatheringComponent. Внутри проекта я прокомментировал эти функции, если вам покажется проблематичным, как передать компонент.  
![Интерфейс](https://sun9-54.userapi.com/s/v1/ig2/tT3ni7l34vXggMaeR340sZGMHKW1mjo9ro8S0bVWiPFUqsu8lVgZZ5rkcXI5dVLJfPEybspEKSFAsXrYaIngDpuu.jpg?quality=95&as=32x15,48x22,72x34,108x51,160x75,240x112,360x169,480x225,540x253,640x300,651x305&from=bu&cs=651x0)  
4. Добавьте DT_Gathering_System_GameplayTags в настройки проекта/GameplayTags/Список таблиц игровых тегов.
![Интерфейс](https://sun9-2.userapi.com/s/v1/ig2/4WIt1mdSool4I1nInlGoVG6GktYuRww3_-mFNWUE66GFcnUL5Er8pkvV0VO7mttvRsajVAK5H472mAV1_HfAHYUt.jpg?quality=95&as=32x5,48x7,72x11,108x16,160x24,240x36,360x54,480x72,540x81,596x89&from=bu&cs=596x0)  
5. Если у вас есть свой собственный персонаж с AnimationBlueprint, скопируйте AnimNotifies из ABP, подключенного к DemoCharacter, в свой AnimationBP.
![Интерфейс](https://sun9-9.userapi.com/s/v1/ig2/qrRk9s9by5wXDBGuhCmTXbQx7x7_imNTUIhpKaVZ68K-InKOrqJ2xk72ElZPoO0zXXTFZnWKdLrjx6d7yr4tQ-LM.jpg?quality=95&as=32x9,48x14,72x21,108x32,160x47,240x70,360x105,480x140,540x158,640x187,720x211,1001x293&from=bu&cs=1001x0)
Не забудьте, если у вас есть своя собственная анимация, добавить эти анимационные уведомления в свой монтаж gathering
![Интерфейс](https://sun9-73.userapi.com/s/v1/ig2/MNtrz9dVAXMC3-POsT-GXAunVoESszGJhKZd1V6EtFWm1HsMXHaJXbboEDitAy3J82qHwRPdIlfUHz2sX5LNtnt8.jpg?quality=95&as=32x7,48x11,72x16,108x24,160x35,240x53,360x79,363x80&from=bu&cs=363x0)

6. В компоненте BPAC_GatheringComponent на вкладке Animations убедитесь, что вы правильно настроили гнездо для подключения инструмента. Это гнездо должно совпадать с гнездом в вашей позиции SkeletalMesh, к которому прикреплен инструмент.
![Интерфейс](https://sun9-68.userapi.com/s/v1/ig2/lgdwCqz7n6qEy9n8kR38biLGogneV8Q_oU6va1xDs2RNAPo3FYFxguNSe61QDBj15_P9p3Cm_eMANtdB31Im9fTA.jpg?quality=95&as=32x3,48x5,72x7,108x11,160x16,240x24,360x37,480x49,540x55,588x60&from=bu&cs=588x0)

**EN:**
1. Add BPAC_GatheringComponent to place of your choice (Character or PlayerState).
2. Add Interface (BPI_GetMesh) to your character class and pass skeletal mesh to get Pawn Mesh function. To add Interface you have to select ClassSettings and in right DetailsPanel find Interfaces tab.
![Interface](https://sun9-17.userapi.com/s/v1/ig2/_IjaQQQbi6ah3EDxIEJo-udtrnC4QiacD_bUyBGHbAV4qZxx2DwIwnPC4uBJvKx9fGIZCKy9pDUAu3rldeqxOriV.jpg?quality=95&as=32x5,48x7,72x10,108x16,160x23,240x35,360x52,480x69,540x78,581x84&from=bu&cs=581x0)
3. Add Interface (BPI_GetComponents) to your Character Class and to Player Controller! and pass GatheringComponent to GetGatheringComponent function. Inside project i commented those functions if you find it is problematic how to pass component.
![Interface](https://sun9-54.userapi.com/s/v1/ig2/tT3ni7l34vXggMaeR340sZGMHKW1mjo9ro8S0bVWiPFUqsu8lVgZZ5rkcXI5dVLJfPEybspEKSFAsXrYaIngDpuu.jpg?quality=95&as=32x15,48x22,72x34,108x51,160x75,240x112,360x169,480x225,540x253,640x300,651x305&from=bu&cs=651x0)
4. Add DT_Gathering_System_GameplayTags to Project Settings/GameplayTags/Gameplay Tag Table List.
![Interface](https://sun9-2.userapi.com/s/v1/ig2/4WIt1mdSool4I1nInlGoVG6GktYuRww3_-mFNWUE66GFcnUL5Er8pkvV0VO7mttvRsajVAK5H472mAV1_HfAHYUt.jpg?quality=95&as=32x5,48x7,72x11,108x16,160x24,240x36,360x54,480x72,540x81,596x89&from=bu&cs=596x0)
5. If you have your own character with AnimationBlueprint copy AnimNotifies from the ABP connected to DemoCharacter into your AnimationBP.
![Interface](https://sun9-9.userapi.com/s/v1/ig2/qrRk9s9by5wXDBGuhCmTXbQx7x7_imNTUIhpKaVZ68K-InKOrqJ2xk72ElZPoO0zXXTFZnWKdLrjx6d7yr4tQ-LM.jpg?quality=95&as=32x9,48x14,72x21,108x32,160x47,240x70,360x105,480x140,540x158,640x187,720x211,1001x293&from=bu&cs=1001x0)
Do not forget if you have your own animation to add those anim notifies into your gathering montage
![Interface](https://sun9-73.userapi.com/s/v1/ig2/MNtrz9dVAXMC3-POsT-GXAunVoESszGJhKZd1V6EtFWm1HsMXHaJXbboEDitAy3J82qHwRPdIlfUHz2sX5LNtnt8.jpg?quality=95&as=32x7,48x11,72x16,108x24,160x35,240x53,360x79,363x80&from=bu&cs=363x0)

6. In BPAC_GatheringComponent in Animations tab be sure to set up correct socket to attach the tool. This socket should match the socket in your SkeletalMesh position to which attach the tool.  
![Interface](https://sun9-68.userapi.com/s/v1/ig2/lgdwCqz7n6qEy9n8kR38biLGogneV8Q_oU6va1xDs2RNAPo3FYFxguNSe61QDBj15_P9p3Cm_eMANtdB31Im9fTA.jpg?quality=95&as=32x3,48x5,72x7,108x11,160x16,240x24,360x37,480x49,540x55,588x60&from=bu&cs=588x0)
---

## 🌅 PROJECT OVERVIEW | ОБЗОР ПРОЕКТА

**RU:**
Эта система позволяет разработчикам добавлять множество типов ресурсов с различными уровнями и заклинаниями, а также требованиями к их "сбору", она также управляет инструментами сбора, долговечностью и другими необходимыми взаимодействиями для такого рода деятельности. Кроме того, в продукте есть компонент BonusGame, который может предоставить игроку дополнительные ресурсы. Все было создано с учетом адаптивности и гибкости. Для внедрения и добавления новых функций требуется всего несколько щелчков мыши.
Продукт поддерживает многопользовательскую игру.

**EN:**
This system allows developers to add numerous types of resources, with varying levels and enchantments, as well as requirements to "Gather" them, it also manages gathering tools,durability and other necessary interactions for that sort of activity. Furthermore, the product has a BonusGame component that may provide the player with extra resources. Everything was created with adaptability and flexibility in mind. It only takes a few clicks to implement and add new features.
Product support MULTIPLAYER.

---

## 🎡 Gathering | Сбор

**RU:**
Найдите инструмент и соберите ресурсы

**EN:**
Find the tool and gather resource.

![Gathering](https://i.imgur.com/VhbMStB.gif)

**RU:**
**Бонусная игра**
Выпадает случайным образом во время сбора (шанс можно определить)

**EN:**
**Bonus Game**
Appear randomly while gathering (Chance can be determined)

![Gathering](https://i.imgur.com/0xrOTYc.gif)

---
