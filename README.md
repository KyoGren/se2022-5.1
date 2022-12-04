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
