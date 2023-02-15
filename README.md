# se2022-5.1
Lớp kĩ thuật điện tử và tin học<br>
#Lập trình game casual thể loại match 3 kết hợp trang trí nhà
<h3>Theo đó phần Review này sẽ giới thiệu các thành phần chính về tựa Game Home Decor qua bằng hình ảnh. Còn muốn tìm hiểu rõ hơn các thành phần và ý nghĩa của từng phần trong source code, các bạn có thể đi sâu và nghiên cứu của từng thành viên trong nhóm chúng tôi</h3>
<h1 style="justify:center">Chức năng chính của Game</h1>
<h3>&nbsp&nbspUnity là một game engine đa nền tảng được phát triển bởi Unity Technologies, mà chủ yếu để phát triển video game cho máy tính, consoles và điện thoại. Trước khi bắt đầu tìm hiểu về tựa game, các bạn có thể tìm hiểu một chút về các thành phần cơ bản trong Unity Hub như (branch <a href="https://github.com/KyoGren/se2022-5.1/tree/dinhQuang">dinhQuang</a>): </h3>
<h4>Cửa sổ sences: Hiển thị đối tượng một cách trực quan và có thể kéo thả phóng to thu nhỏ</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/sences.PNG">
<h4>Tab hierarchy: hiển thị các Game object trong sences hiện hành . Khi các đối tượng được thêm hoặc xóa trong sences , tương ứng với các đối tượng có trong hierarchy</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/hierachy.PNG">
<h4>Và vài chức năng đối với từng phần code riêng như: Project Assets (hiển thị thông tin của tất cả các tài nguyên); Inspector (hiện thị thông tin, code về GameObject đang làm việc,...</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/project-asset.PNG">
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/inspector.PNG">
<h2 style="justify:center">1. Trang trí nhà cửa</h2>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Frenceprops_1.png">
<h3>&nbsp&nbspHình ảnh trên cũng là ví dụ cách mà bạn trang trí. Để muốn căn nhà của bạn trở lên đẹp hơn, hào nhoàng hơn bạn có thể lựa chọn 1 trong 3 cách mà bạn muốn mua đối với đồ dùng trong căn nhà theo mong muốn của mình. Cách thức mà đồ trang trí đồ đạc hoạt động như trong source code được tìm hiểu (branch<a href="https://github.com/KyoGren/se2022-5.1/tree/TungNguyen"> TungNguyen</a>)</h3>
<h3>&nbsp&nbspNhưng bạn không thể mua mọi thứ miễn phí được, mỗi vật phẩm được lựa chọn sẽ tiêu tốn những tài nguyên nhất định. Các tài nguyên đó được coi như một loại tiền ảo như star, coin. Các đối tượng trên chủ yếu nằm trong phần CurrencyPanel (brach<a href="https://github.com/KyoGren/se2022-5.1/tree/TuanDo"> TuanDo</a>): </h3>
<h4>Star: số lần cho phép trang trí</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/StarsCurrency/1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/StarsCurrency/2.png">
<h4>Live: thực hiện hiển thị số mang (số lượt chơi)</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/LivesCurrency/1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/LivesCurrency/2.png">
<h4>Coin</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/2.png">
<h5>Đối với coin, các bạn có thể mua thêm coin để đấy nhanh tiến độ trang trí mà mình muốn bằng cách mua chúng tại cửa hàng. Trong cửa hàng thì có những chức năng cơ bản như: + nút hủy để trở về cảnh trò chơi thiết kế nhà + nhấn vào hàng hóa để thực hiện mua hàng (hiện tại thì khi ấn vào nút mùa xanh thì không thực hiện mua hàng mà phải ấn vào đối tượng BigOfferPrefabBlue(cảnh)) + nút chuyển trang hiển thị thêm nhiều sản phẩm hơn</h5>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/3.png">
<h5>Hiện thị sản phẩm tại của hàng</h5>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/7.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/8.png">
<h3>&nbsp&nbsp Để trải nghiệm đầy đủ nhất, tựa game được thêm các chức năng như:</h3>
<h4>&nbsp&nbsp + Button Home: lựa chọn màn chơi (brach AnhQuan)</h4>
<h4>&nbsp&nbsp + Setting: Thiết lập mức độ âm thanh và nhạc (branch TuanDo)</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_2_HomeButton.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/1.jpg">
<h3>Thiết kế trang trí sẽ không bị giới hạn ở một màn chơi duy nhất, các Room khác sẽ được mở khóa khi bắt đã hoàn thành màn chơi đầu tiên. Chức năng này cho phép bạn đổi màn chơi của mình để tiếp tục trang trí những thứ khác trong ngôi nhà của mình. Nút Home được đặt tại vị trí(x, y) = (66, 63,75) trên màn hình hiển thị, có chiều dài và chiều rộng(height, width) = (106, 106) </h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_1_Tongquan.png">
<h3>Sau khi thực hiện thao tác nhấn, giao diện người dùng được chuyển tới màn hình lựa chọn phòng chơi(Room). Nhưng chúng thường sẽ chỉ mở khóa khi bạn trang trí đầy đủ tất cả map trước đó</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_3_ScrollableSelectRoomScreen.png">
<h3>Các Room chưa được mở khóa và điều kiện mở khóa Room</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_7_RoomLocked.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_8_RoomPass.png">
<h3>Nút bấm Setting có tác dụng để bạn điều chỉnh nhạc và mức độ âm thanh của trò chơi. Nó nằm ngay bên trên Button Home</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/1.jpg">
<h3>Trong InGameSettingsScreen có nút thoát , nút chỉnh âm thanh, nhạc hoạt động với các chức năng thoát trở về màn hình chính, thay đổi tắt bật âm thanh, âm nhạc</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/3.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/4.jpg">
<h3> Khi hoàn thành những thay đổi thiết lập của bạn, nhấn nút X sẽ gọi đến hàm OnExit để chuyển về màn hình chính. Nhấn tắt bật âm thanh sẽ gọi đến hàm OnClick để thay đổi trạng thái và cập nhật lại trên trò chơi</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/4.jpg">
<h3>Bạn sẽ trang trí bằng ngôi sao kiếm được thông qua mỗi khi vượt qua vòng chơi GameMatch3. Khi đó vật trang trí sẽ được khởi tạo và một ngôi sao bị mất. Mỗi phần trang trí đều có 3 lựa chọn để thay đổi (brach TungNguyen)</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Frenceprops_1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Door_2.png">
<h3>Còn nếu bạn khổng đủ ngôi sao, hàm điều kiện kiểm tra sẽ đưa đến cấu trúc yêu cầu chơi game</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Not_Enough_Star.png">
<h3>Các điều kiện để có thể trang trí được hay không hay khởi tạo màn hình chơi game mới có thể trang trí đều nằm trong function MoveNext() bằng cách kiểm tra int num = this._003C_003E1__state chính là số ngôi sao hiện có. Nếu != 0 thì cho phép trang trí và số ngôi sao -1, ngược lại set một khu vực có cấu trúc trên</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_MoveNext.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Code/DecorateScene_MoveNext2.png">
<hr/>
<h2 style="justify:center">2. Match 3 Gameplay</h2>
<h3>&nbsp&nbsp Vậy cách thức nào khiến bạn kiếm được những tài nguyên để bắt đầu trang trí. Trò chơi bắt đầu khi bạn nhất vào Button Play để bắt đầu vào game. Match 3 Game là trò chơi video xếp hình là một loại trò chơi điện tử giải đố trong đó người chơi điều khiển các ô xếp để làm cho chúng biến mất theo một tiêu chí phù hợp. Trong nhiều trò chơi ghép ô, tiêu chí đó là đặt một số ô nhất định cùng loại sao cho chúng liền kề nhau. Button được tìm hiểu tại branch<a href="https://github.com/KyoGren/se2022-5.1/tree/NguyenTrung"> NguyenTrung</a></h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/NguyenTrung/Img/ButtonPlay.png">
<h3>Khi bạn nhấn vào Button PlayGame, một cửa sổ PreGame sẽ được khởi tạo. Trong đó có chứa các khả năng đặc biệt để bắt đầu màn chơi, điều đó sẽ khiến bạn thấy bớt khó khăn hơn nếu muốn qua màn. Hoặc chỉ đơn giản là tắt nó đi để quay lại trang trí ngôi nhà</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/NguyenTrung/Img/PregameScreen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/NguyenTrung/Img/PlayButtonclick.png">
<h3>Ở màn hình Pregame có nút play, nếu bấm vào thì chúng ta sẽ vào được màn chơi đó được tạo  ButtonCallback_OnPlayButtonClick</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/NguyenTrung/Img/ButtonCallback_OnPlayButtonClickedcode.png">
<h3>Nhiệm vụ đơn giản của các tự game dạng Match3 là di chuyển thành các hàng hoặc cột gồm 3 khối block giống hệt nhau. Khi đó thì các block sẽ biến mất và các block sẽ rơi xuống(branch TungNguyen)</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/Move1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/Move2.png">
<h3> Theo đó phần code đễ di chuyển các khối block chủ yếu dựa vào engine có săn để tích hợp với màn hình điện thoại. Quá trinh đó bao gồm 2 bước là TrySwitchSlot và TapOnSlot. TapOnSlot có hàm powerupsUseByTap chính là cách bạn nhấn vào màn hình và chọn khối block mà bạn muốn</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/TapOnSlot.png">
<h3>Còn Switch slot chính là cấu trúc để bạn có thể tráo đổi 2 khối block với nhau</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3/Code_Match3/Swtich_slot.png">
<h3>Ngoài việc cách kết hợp 3 khối block thành một hàng hoặc cột để hoàn thành vòng chơi, trò chơi được thêm vào các khối block đặc biệt. Tuy nhiên yêu cầu để tạo ra chúng cũng khó khăn hơn việc di chuyển block thông thường. Các khối block này khiến cho trò chơi vui vẻ hơn rất nhiều (brach TungNguyen): </h3>
<h4>- Cross Bomb: được tạo ra khi các khối block có kết hợp theo hình dạng dấu cộng</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/CrossBomb/Before_Cross_Bom.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/CrossBomb/Done_Cross_Bom.png">
<h4>- HorizonRocket: được khởi tạo khi di chuyển block thành một hàng ngang gồm 4 block trùng nhau</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/HorizonRocket/Before_HorizonRocket.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/HorizonRocket/Done_HorizonRocket.png">
<h4>- VerticalRocket: Tương tự như HorizonRocket nhưng theo hàng dọc</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/VerticalRocket/Before_VerticalRocket.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/VerticalRocket/Done_VerticalRocket.png">
<h4>- SeekingMissle: được tạo ra khi kết hợp thành 4 block hình vuông</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/SeekingMissle/Before_SeekingMissle.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/SeekingMissle/Done_SeekingMissle.png">
<h4>-DiscoBall: được tạo ra khi kết hợp 5 khối block giống nhau</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/DiscoBall/Before_Bomb5.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Single_Affect/DiscoBall/Done_Bomb5.png">
<h3> Đặc biệt hơn là các hiệu ứng mạnh mẽ khí 2 khối block đặc biệt được kết hợp với nhau. Sức phả hủy lớn có thể giúp bạn hoàn thành mục tiêu dễ dàng hơn rất nhiều. Việc gồm 5 block đặc biệt và chúng có thể kết hợp giống nhau nên có ít nhất 25 trường hợp có thể xảy ra, vì vậy tôi sẽ chỉ đưa ra một vài ví dụ:<h/3>
<h4>VerticalRocket + SeekingMissle: lần này tại vị trí máy bay bay đến, sẽ quét sách một hàng ngang</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Before_VerticalRocket_%26_SeekingMissle.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Active_VerticalRocket_%26_SeekingMissle.png">
<h4>HorizonRocket/VerticalRocket + CrossBomb: Sẽ quét sạch cả 3 hàng ngang và dọc</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Before__HorizonRocket_%26_CrossBomb.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Img/Double_Affect/Active__HorizonRocket_%26_CrossBomb.png">
<h4>SeekingMissle + CrossBomb: lần này tại vị trí máy bay bay đến, sẽ nổ với kích thước như CrossBomb</h4>
<h3> Các cách thức trên được kết hợp dựa vào một function kết hợp. Một List combines bao gồm CombineType khác nhau được khởi tạo tại Line 2563. Ở đó được set điều kiện đối với có thể kết hợp với các CombineType khác nhau hoặc Double[CombineType]. Hàm SelecPotentialMatch Line 2611 là hàm di chuyển chính để xác nhận chúng đã Match với nhau</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Match3Gameplay/M3G_Code/Combine.png">
<h3> meunu thoát game (branch TuanDo)</h3>
<p> Bằng việc bấm vào nút răng cưa hiển thị thanh hiện nút exit bấm vào kích hoạt thông của sổ thông báo và thoát trở về màn hình game decor</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/5.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/6.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/7.jpg">
<hr/>
<h2 style="justify:center">3. Ý tưởng thiết kế Button Reset Decorate</h2>
<h3>&nbsp&nbsp Nhóm chúng tôi muốn tạo nên một ý tưởng thiết kế một Button khiến những trang trí của bạn trước đó khởi tạo lại để giúp bạn thay thế toàn bộ về màn chờ ban đầu. Tất nhiên ban sẽ được trả lại những ngôi sao bạn đã dùng để làm điều đó. Chúng tôi đã tạo một Project để cả nhóm vào góp ý để hiểu rõ hơn về source code. Nếu muốn tìm hiểu bạn có thể đi vào đường liên kết của dự án https://github.com/KyoGren/se2022-5.1/issues/53</h3>
<img src="https://user-images.githubusercontent.com/95405402/214495079-1c9e90fc-3a83-4769-adf1-c18cec05948c.png">
<h3>Add Component hoạt động cần tạo hàm Reset trong File DecoratingScene và DecoratingSceneConfig. Trong đó Scene là file chứa hàm và SceneConfig chủ yếu là hiện thị các thành phần trong Map</h3>
<img src="https://user-images.githubusercontent.com/95405402/214494922-f3286375-ce99-462f-b044-b075f0977e8f.png">
</hr>
<<h2 style="justify:center">Extra: một vài chức năng phụ</h2>
<h3>&nbsp&nbsp + Màn hình chờ trước khi bắt đầu Game (branch TungNguyen)</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartImg/Start_Screen.png">
<h3>Các hàm bên dưới sẽ được thiết lập thêm để <b>"Hide"</b> màn hình hiện tại và <b>"Show"</b> phần khởi chạy của đổi tượng tiếp theo</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Load_Push_Screen.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/StartCode/Setup_Code.png">
<h3>&nbsp&nbsp + Màn hình chờ trước khi bắt đầu Match 3 Game (brach NguyenTrung)</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/NguyenTrung/Img/Itemselect.jpg">
  
