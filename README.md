# se2022-5.1
<h1 style="justify:center">1. Ngiên cứu hiện thì màn hình khởi đầu khi vào Game</h1>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartImg/Start_Screen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/StartScreen_Position.png">
<h3>Lần đầu tiên chạy chương trình thì màn hình hiện tại (currentScreen) sẽ được Awake khởi tạo</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Load_Start_Screen_Code.png">
<h3>Khi đó màn hình bắt đầu game sẽ được khởi tạo bởi LoadStartLayer và Push</h4>
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
<h3>Các điều kiện để có thể trang trí được hay không hay khởi tạo màn hình chơi game mới có thể trang trí đều nằm trong function MoveNext() bằng cách kiểm tra int num = this._003C_003E1__state chính là số ngôi sao hiện có. Nếu != 0 thì cho phép trang trí và số ngôi sao -1, ngược lại set một khu vực có cấu trúc trên</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_MoveNext.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_MoveNext2.png">

<h1 style="justify:center">3. Ngiên cứu di chuyển các khổi block và cách kết hợp thành block đặc biệt trong Match3 Gameplay</h1>
<h2> 3.1 Cách di chuyển các khối block
<h3>Như cái tên của mình, nhiệm vụ đơn giản của các tự game dạng Match3 là di chuyển thành các hàng hoặc cột gồm 3 khối block giống hệt nhau. Khi đó thì các block sẽ biến mất</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/Move1.png">
<h3>Khi di chuyển thì các khối block đạt điều kiện như đã nói bên trên sẽ biến mất. Khi đó vị trí cũ của chúng sẽ biến mất và các khối block phía bên trên sẽ rơi xuống</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/Move2.png">
<h3> Theo đó phần code đễ di chuyển các khối block chủ yếu dựa vào engine có săn để tích hợp với màn hình điện thoại. Quá trinh đó bao gồm 2 bước là TrySwitchSlot và TapOnSlot. TapOnSlot có hàm powerupsUseByTap chính là cách bạn nhấn vào màn hình và chọn khối block mà bạn muốn</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/TapOnSlot.png">
<h3>Còn Switch slot chính là cấu trúc để bạn có thể tráo đổi 2 khối block với nhau</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/Swtich_slot.png">
<h2> 3.2 Các khối block đặc biệt</h2>
<h3>Ngoài việc cách kết hợp 3 khối block thành một hàng hoặc cột để hoàn thành vòng chơi, trò chơi được thêm vào các khối block đặc biệt. Tuy nhiên yêu cầu để tạo ra chúng cũng khó khăn hơn việc di chuyển block thông thường. Các khối block này khiến cho trò chơi vui vẻ hơn rất nhiều: </h3>
<h4>- Cross Bomb: được tạo ra khi các khối block có kết hợp theo hình dạng dấu cộng</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/CrossBomb/Before_Cross_Bom.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/CrossBomb/Done_Cross_Bom.png">
<h4>Bạn sẽ cần một lượt nữa để kích nổ CrossBomb. Khi đó một khu vực nhỏ sẽ nổ và xóa sạch các block ở đó<h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/CrossBomb/Active_Cross_Bom.png">
<h4>Hàm khởi tạo CrossBomb và nguyên lý nằm ở phần code bên dưới</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Cross_Area.png">
<h4>- HorizonRocket: được khởi tạo khi di chuyển block thành một hàng ngang gồm 4 block trùng nhau</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/HorizonRocket/Before_HorizonRocket.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/HorizonRocket/Done_HorizonRocket.png">
<h4>Khi được active (khi bạn nhấn vào màn hình điện thoại hoặc di chuyển nó với block khác) thì một hàng dọc sẽ bị xóa</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/HorizonRocket/Active_HorizonRocket.png">
<h4>Hàm khởi tạo HorizonRocket và nguyên lý nằm ở phần code bên dưới</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Horizon_Area.png">
<h4>- VerticalRocket: Tương tự như HorizonRocket nhưng theo hàng dọc
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/VerticalRocket/Before_VerticalRocket.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/VerticalRocket/Done_VerticalRocket.png">
<h4>Khi được active (khi bạn nhấn vào màn hình điện thoại hoặc di chuyển nó với block khác) thì một hàng ngang sẽ bị xóa</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/VerticalRocket/Active_VerticalRocket.png">
<h4>Hàm khởi tạo HorizonRocket và nguyên lý nằm ở phần code bên dưới</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Vertical_Area.png">
<h4>- SeekingMissle: được tạo ra khi kết hợp thành 4 block hình vuông</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/SeekingMissle/Before_SeekingMissle.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/SeekingMissle/Done_SeekingMissle.png">
<h4>Khi được active (khi bạn nhấn vào màn hình điện thoại hoặc di chuyển nó với block khác) chiếc may bay sẽ nổ ra dấu cộng nhỏ tại vị trí của nó và bay tới phá hủy một block khác. Vị trí bay tới thường ưu tiên với nhiệm vụ</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/SeekingMissle/Active_SeekingMissle.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/SeekingMissle_Area.png">
<h4>-DiscoBall: được tạo ra khi kết hợp 5 khối block giống nhau</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/DiscoBall/Before_Bomb5.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/DiscoBall/Done_Bomb5.png">
<h4>DiscoBall chỉ active khi kết hợp với một block khác. Nó sẽ phá hủy các block giống như block đã chọn</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/DiscoBall/Active_Bomb5.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Bomb5_Destroy.png">
<h3>Các khối block trên được trả về ứng với biến chipType và vị trí centerPos chính là vị trí block di chuyển chính mà các bạn đảo vị trí</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Return_Bomb.png">
<h2> 3.3 Kết hợp các khôi block đặc biệt với nhau
<h3> Đặc biệt hơn là các hiệu ứng mạnh mẽ khí 2 khối block đặc biệt được kết hợp với nhau. Sức phả hủy lớn có thể giúp bạn hoàn thành mục tiêu dễ dàng hơn rất nhiều. Việc gồm 5 block đặc biệt và chúng có thể kết hợp giống nhau nên có ít nhất 25 trường hợp có thể xảy ra, vì vậy tôi sẽ chỉ đưa ra một vài ví dụ:<h/3>
<h4>VerticalRocket + SeekingMissle: lần này tại vị trí máy bay bay đến, sẽ quét sách một hàng ngang</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Before_VerticalRocket_%26_SeekingMissle.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Active_VerticalRocket_%26_SeekingMissle.png">
<h4>HorizonRocket/VerticalRocket + CrossBomb: Sẽ quét sạch cả 3 hàng ngang và dọc</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Before__HorizonRocket_%26_CrossBomb.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Active__HorizonRocket_%26_CrossBomb.png">
<h4>SeekingMissle + CrossBomb: lần này tại vị trí máy bay bay đến, sẽ nổ với kích thước như CrossBomb</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Before_SeekingMissle%26CrossBomb.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Active_SeekingMissle%26CrossBomb.png">
<h4>DiscoBall + DiscoBall: Quét sạch các khối block trong màn chơi</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Before_Bomb5_Bomb5.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Active_Bomb5_Bomb5.png">

<h3> Các cách thức trên được kết hợp dựa vào một function kết hợp. Một List combines bao gồm CombineType khác nhau được khởi tạo tại Line 2563. Ở đó được set điều kiện đối với có thể kết hợp với các CombineType khác nhau hoặc Double[CombineType]. Hàm SelecPotentialMatch Line 2611 là hàm di chuyển chính để xác nhận chúng đã Match với nhau</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Combine.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Combine_Move.png">

