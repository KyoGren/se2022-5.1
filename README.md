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
<h3>Theo đó với ví dụ Map Veranda được khởi tạo các hình ảnh ở Assets/Scripts/Sprites được khởi tạo khi trò chơi chạy (MainUI hoạt động). Khi đó các function của từng hình ảnh muốn chèn sẽ được khởi tạo tại Room0090_Veranda_First. Các đặc tính với ví dụ minh họa trang trí đầu tiên fenceprops sẽ được hiểnn thị bên dưới</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Decorate_Eg.png">
<h3>Các vị trí bản có thể trang trí tạo những nơi đang có ngôi sao dấu + trên màn chơi. Vị trí này được thực hiện bằng code CharacterBubblePosition trong file DecorateScene.cs. Khi bắt đầu trang trí sẽ có kết quả như bên dưới</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Decorate_Eg2.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Door_1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_Position.png">
<h3>Theo đó, các đặc tính của một vật trang trí gồm Groupname và hoạt ảnh Amination</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_GroupDef.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_setCharacter_%26_Animation.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_setCharacter_%26_Animation_All.png">
<h3> Các phần trang trí sẽ được đếm và đưa thành một List visualObjectBehaviour và sẽ hiện thị qua function ShowAll()</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_Show_Config.png">

<h3>Bạn sẽ trang trí bằng ngôi sao kiếm được thông qua mỗi khi vượt qua vòng chơi GameMatch3. Khi đó vật trang trí sẽ được khởi tạo và một ngôi sao bị mất. Mỗi phần trang trí đều có 3 lựa chọn để thay đổi. Bên dưới là vị dụ minh họa</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Frenceprops_1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Door_2.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_Update.png">
<h3>Còn nếu bạn khổng đủ ngôi sao, hàm điều kiện kiểm tra sẽ đưa đến cấu trúc yêu cầu chơi game</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Not_Enough_Star.png">
<h3>Các điều kiện để có thể trang trí được hay không hay khởi tạo màn hình chơi game mới có thể trang trí đều nằm trong function MoveNext()</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_MoveNext.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_MoveNext2.png">
