# se2022-5.1
<h1 style="justify:center">1. Ngiên cứu hiện thì màn hình khởi đầu khi vào Game</h1>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartImg/Start_Screen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/StartScreen_Position.png">
<h3>lần đầu tiên chạy chương trình thì màn hình hiện tại (currentScreen) sẽ được Awake khởi tạo</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Load_Start_Screen_Code.png">
<h3>Khi đó màn hình bắt đầu game sẽ được khởi tạo bởi LoadStartLayer và Push</h3>
<h3>Các hàm bên trên sẽ được thiết lập thêm để <b>"Hide"</b> màn hình hiện tại và <b>"Show"</b> phần khởi chạy của đổi tượng tiếp theo</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Load_Push_Screen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Setup_Code.png">
<h3>Khi đó màn hình load sẽ được đẩy vào thành CurrentScreen và thực hiện Load trước khi vào Game</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartImg/LoadingScreen.png">
<h3>Ngoài ra khi thoát khỏi App cần code để Screen sẽ khởi chạy lại được thiết kế trong <b>"SplashScreen"</b></h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/NewScreen_After_Quit_Code.png">

<h1 style="justify:center">2. Ngiên cứu trang trí map bằng ngôi sao nhận được</h1>
<h3>Theo đó với ví dụ Map Veranda được khởi tạo các hình ảnh ở Assets/Scripts/Sprites được khởi tạo khi trò chơi chạy (MainUI hoạt động). Khi đó các function của từng hình ảnh muốn chèn sẽ được khởi tạo tại Room0090_Veranda_First. Các đặc tính sẽ được hiện thị bên dưới</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Decorate_Eg.png">
