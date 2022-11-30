# se2022-5.1
<h1 style="justify:center">Ngiên cứu hiện thì màn hình khởi đầu khi vào Game</h1>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartImg/Start_Screen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/StartScreen_Position.png">
<h3>lần đầu tiên chạy chương trình thì màn hình hiện tại (currentScreen) sẽ được Awake khởi tạo</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Load_Start_Screen_Code.png">
<h3>Khi đó màn hình bắt đầu game sẽ được khởi tạo bời LoadStartLayer và Push</h3>
<h3>Các hàm bên trên sẽ được thiết lập thêm để <b>"Hide"</b> màn hình hiện tại và <b>"Show"</b> phần khởi chạy của đổi tượng tiếp theo</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Load_Push_Screen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Setup_Code.png">
<h3>Ngoài ra khi thoát khỏi App cần code để Screen sẽ khởi chạy lại được thiết kế trong <b>"SplashScreen"</b></h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/NewScreen_After_Quit_Code.png">
