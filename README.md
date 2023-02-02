# se2022-5.1
<h1 style="justify:center">Nghiên cứu label hiển thị số ngôi sao</h1>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/StarsCurrency/1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/StarsCurrency/2.png">
<h3>lần đầu tiên chạy chương trình sẽ hủy các đối tượng được tạo ra và thay đổi số ngôi sao bằng count  khởi tạo</h3>
<h3>hàm displaycount để hiển thị số ngôi sao bằng cách sử dụng hàm thay đổi text để thay đổi đối tượng text mesh pro là countLabel</h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/StarsCurrency/3.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/StarsCurrency/4.png">
<h1 style="justify:center;">Nghiên cứu label hiển thị số tiền</h1>
<h3>giống với khi thực hiện với trái ngôi sao do dùng chung 1 file mã <b>"CurrencyDisplay"</b></h3>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/2.png">
<h3> add coin</h3>
<p>nhấn dấu cộng thực hiện gọi file script để thực hiện chức năng chuyển đến cảnh CurrencyPurchaseDialog để hiển thị chỗ để mua hàng <p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/4.png">
<p>
trong cảnh mua hàng thì có những chức năng cơ bản như:
	+ nút hủy để trở về cảnh trò chơi thiết kế nhà
	+ nhấn vào hàng hóa để thực hiện mua hàng (hiện tại thì khi ấn vào nút mùa xanh thì không thực hiện mua hàng mà phải ấn vào đối tượng BigOfferPrefabBlue(cảnh))
	+ nút chuyển trang hiển thị thêm nhiều sản phẩm hơn
</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/3.png">
<p>khi gọi file script currencyPurchaseDialog,tại hàm Init() (hàm khi chạy file được sinh ra) chạy hàm Init(offers,onHide,type) để khởi tạo và cài đặt các chức năng trong cảnh </p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/6.png">
<p>Đoạn code lấy dữ liệu sản phẩm ra và thêm vào danh sách sản phẩm để hiển thị trên cảnh 
	+ với danh sách 1 ( đối tượng list) để hiển thị tại page 1
	+ với danh sách 2 ( đối tượng list2) để hiển thị tại page 2 sau khi nhấn nút chuyển tiếp ">>"</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/7.png">
<p>Đoạn code để quy định số lượng sản phẩm hiển thị tại các trang</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/8.png">
<p>Khi nhấn mua hàng thì thực hiện animation làm tối nền rồi lấy thông tin sản phẩm và thực hiện chuyển cảnh để mua hàng</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/9.png">
<p>nhấn vào button NextButtonPrefab thực hiện chuyển tiếp sang trang 2 (page 2)</p>
<p>hàm thực hiện quay trở lại cảnh trò chơi</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/CoinCurrency/10.png">
<h1>LiveCurrency</h1>
<p> thực hiện hiển thị số mang (số lượt chơi). mạng sẽ giảm đi khi thất bại màn chơi game match3 và sẽ phải chờ thời gian hồi</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/LivesCurrency/1.png">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/LivesCurrency/2.png">

<hr>
<h1> Tìm hiểu về nút setting</h1>
<p>Khi nhấn vào nút setting nó sẽ gọi kiểm tra trong cảnh DecorateRoomScreen gọi đến hàm OnSettingsButtonPress để chuyển sang cảnh InGameSettingsScreen<p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/1.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/2.jpg">
<p> Trong cảnh InGameSettingsScreen có nút thoát , nút chỉnh âm thanh, nhạc hoạt động với các chức năng thoát trở về màn hình chính, thay đổi tắt bật âm thanh, âm nhạc</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/3.jpg">
<p> Khi nhấn nút X sẽ gọi đến hàm OnExit để chuyển về màn hình chính</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/4.jpg">
<p> Nhấn tắt bật âm thanh sẽ gọi đến hàm OnClick để thay đổi trạng thái và cập nhật lại trên trò chơi</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/5.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/6.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/7.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/ButtonSetting/8.jpg">
<hr>
<h1> Màn hình chơi trong game match3</h1>
<p> Trong sence GameScreen -> sence GoalsPanel -> content là hiển thị thanh cấp độ, điều kiện để qua màn và số nước đi tối đa</p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/1.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/2.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/3.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/4.jpg">
<p> Sau mỗi khi chơi thì số lượt sẽ giảm đi và nếu ăn được đúng loại chip thì điều kiện sẽ trừ đi, khi đk hết mà vẫn còn lượt thì sẽ qua màn còn ko sẽ thất bại</p>
<h1> meunu thoát game</h1>
<p> bằng việc bấm vào nút răng cưa hiển thị thanh hiện nút exit bấm vào kích hoạt thông của sổ thông báo và thoát trở về màn hình game decor</h1>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/5.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/6.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/7.jpg">
<h1> game play and event </h1>
<p> Các chip khi được match với nhau mà đúng thì sẽ xảy ra sự kiện như kích hoạt animation, biến mất thay đổi thành các sự kiện như bom, đồng thời sinh ra các chip mới, màu sác mới thay thế chỗ các chip đã biến mất </p>
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/16.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/15.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/14.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/13.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/12.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/11.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/10.jpg">
<img src="https://github.com/KyoGren/se2022-5.1/blob/TuanDo/gameScreen/9.jpg">
