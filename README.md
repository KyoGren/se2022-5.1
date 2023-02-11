# se2022-5.1
Lớp kĩ thuật điện tử và tin học<br>
#Lập trình game casual thể loại match 3 kết hợp trang trí nhà
<h3>Theo đó phần Review này sẽ giới thiệu các thành phần chính về tựa Game Home Decor qua bằng hình ảnh. Còn muốn tìm hiểu rõ hơn các thành phần và ý nghĩa của từng phần trong source code, các bạn có thể đi sâu và nghiên cứu của từng thành viên trong nhóm chúng tôi</h3>
<h1 style="justify:center">Chức năng chính của Game</h1>
<h3>&nbsp&nbspUnity là một game engine đa nền tảng được phát triển bởi Unity Technologies, mà chủ yếu để phát triển video game cho máy tính, consoles và điện thoại. Trước khi bắt đầu tìm hiểu về tựa game, các bạn có thể tìm hiểu một chút về các thành phần cơ bản trong Unity Hub như: </h3>
<h4>Cửa sổ sences: Hiển thị đối tượng một cách trực quan và có thể kéo thả phóng to thu nhỏ</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/sences.PNG">
<h4>Tab hierarchy: hiển thị các Game object trong sences hiện hành . Khi các đối tượng được thêm hoặc xóa trong sences , tương ứng với các đối tượng có trong hierarchy</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/hierachy.PNG">
<h4>Và vài chức năng đối với từng phần code riêng như: Project Assets (hiển thị thông tin của tất cả các tài nguyên); Inspector (hiện thị thông tin, code về GameObject đang làm việc,...</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/project-asset.PNG">
<img src="https://github.com/KyoGren/se2022-5.1/blob/dinhQuang/unity_component/inspector.PNG">
<h2 style="justify:center">1. Trang trí nhà cửa</h2>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TungNguyen/Decorate/Decorate_Img/Frenceprops_1.png">
<h3>&nbsp&nbspHình ảnh trên cũng là ví dụ cách mà bạn trang trí. Để muốn căn nhà của bạn trở lên đẹp hơn, hào nhoàng hơn bạn có thể lựa chọn 1 trong 3 cách mà bạn muốn mua đối với đồ dùng trong căn nhà theo mong muốn của mình. Cách thức mà đồ trang trí đồ đạc hoạt động như trong source code được tìm hiểu trong branch TungNguyen</h3>
<h3>&nbsp&nbspNhưng bạn không thể mua mọi thứ miễn phí được, mỗi vật phẩm được lựa chọn sẽ tiêu tốn những tài nguyên nhất định. Các tài nguyên đó được coi như một loại tiền ảo như star, coin. Các đối tượng trên chủ yếu nằm trong phần CurrencyPanel: </h3>
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
<h4>&nbsp&nbsp + Button Home: lựa chọn màn chơi</h4>
<h4>&nbsp&nbsp + Setting: Thiết lập mức độ âm thanh và nhạc</h4>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_2_HomeButton.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/1.jpg">
<h3>Thiết kế trang trí sẽ không bị giới hạn ở một màn chơi duy nhất, các Room khác sẽ được mở khóa khi bắt đã hoàn thành màn chơi đầu tiên. Chức năng này cho phép bạn đổi màn chơi của mình để tiếp tục trang trí những thứ khác trong ngôi nhà của mình. Nút Home được đặt tại vị trí(x, y) = (66, 63,75) trên màn hình hiển thị, có chiều dài và chiều rộng(height, width) = (106, 106) </h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_1_Tongquan.png">
<h3>Sau khi thực hiện thao tác nhấn, giao diện người dùng được chuyển tới màn hình lựa chọn phòng chơi(Room). Nhưng chúng thường sẽ chỉ mở khóa khi bạn trang trí đầy đủ tất cả map trước đó</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/AnhQuan/HomeButton/Pic_3_ScrollableSelectRoomScreen.png">
<h3>Nút bấm Setting có tác dụng để bạn điều chỉnh nhạc và mức độ âm thanh của trò chơi. Nó nằm ngay bên trên Button Home</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/1.jpg">
<h3>Trong InGameSettingsScreen có nút thoát , nút chỉnh âm thanh, nhạc hoạt động với các chức năng thoát trở về màn hình chính, thay đổi tắt bật âm thanh, âm nhạc</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/3.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/4.jpg">
<h3> Khi hoàn thành những thay đổi thiết lập của bạn, nhấn nút X sẽ gọi đến hàm OnExit để chuyển về màn hình chính. Nhấn tắt bật âm thanh sẽ gọi đến hàm OnClick để thay đổi trạng thái và cập nhật lại trên trò chơi</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/4.jpg">
<hr/>
<h2 style="justify:center">2. Match 3 Gameplay</h2>
<h3>&nbsp&nbsp Vậy cách thức nào khiến bạn kiếm được những tài nguyên để bắt đầu trang trí. Trò chơi bắt đầu khi bạn nhất vào Button Play để bắt đầu vào game. Match 3 Game là trò chơi video xếp hình là một loại trò chơi điện tử giải đố trong đó người chơi điều khiển các ô xếp để làm cho chúng biến mất theo một tiêu chí phù hợp. Trong nhiều trò chơi ghép ô, tiêu chí đó là đặt một số ô nhất định cùng loại sao cho chúng liền kề nhau. Button được tìm hiểu tại branch NguyenTrung</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/NguyenTrung/Img/ButtonPlay.png">
<h3>&nbsp&nbsp Nguyên lý trò chơi: Thiếu -----------------------------------------------------</h3>
<hr/>
<h2 style="justify:center">3. Ý tưởng thiết kế Button Reset Decorate</h2>
<h3>&nbsp&nbsp Nhóm chúng tôi muốn tạo nên một ý tưởng thiết kế một Button khiến những trang trí của bạn trước đó khởi tạo lại để giúp bạn thay thế toàn bộ về màn chờ ban đầu. Tất nhiên ban sẽ được trả lại những ngôi sao bạn đã dùng để làm điều đó. Chúng tôi đã tạo một Project để cả nhóm vào góp ý để hiểu rõ hơn về source code. Nếu muốn tìm hiểu bạn có thể đi vào đường liên kết của dự án https://github.com/KyoGren/se2022-5.1/issues/53</h3>
</hr>
<<h2 style="justify:center">Extra: một vài chức năng phụ</h2>
<h4>&nbsp&nbsp + Màn hình chờ trước khi bắt đầu Game tại branch TungNguyen</h4>
<h4>&nbsp&nbsp+ Màn hình chờ trước khi bắt đầu Match 3 Game tại branch TrungNguyen</h4>
  
