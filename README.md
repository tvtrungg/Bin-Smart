# Bin-Smart
Thùng rác thông minh là một sản phẩm công nghệ hiện đại tích hợp nhiều tính năng đáng chú ý như phân loại rác, tự động hóa các quy trình xử lý và đảm bảo vệ sinh môi trường. Khi người sử dụng tiến đến, khoảng cách 5cm - 10cm, cảm biến hồng ngoại sẽ kích hoạt nắp thùng để người dùng bỏ rác và đóng nắp kín sau khi hoàn tất. Hình ảnh rác được ghi lại bởi camera và thông qua việc sử dụng công nghệ Machine Learning, các loại rác sẽ được phân loại và rơi vào ô chứa tương ứng. Khi thùng rác đầy, loa tích hợp sẽ cảnh báo người dùng để đưa rác đi đổ. Thùng rác thông minh được trang bị một ESP8266 để kết nối wifi, nhưng trong tình hình dịch bệnh, MQTT Explorer có thể được sử dụng để giả lập ESP8266 và kết nối với NodeRED và MQTT.

Bản vẽ bên ngoài

![image](https://user-images.githubusercontent.com/101247575/225342699-3fa95e2a-3a2e-4809-a566-343e7b4f9562.png)
![image](https://user-images.githubusercontent.com/101247575/225342827-63e646e4-7975-481d-ba3b-f5741000cbf3.png)
![image](https://user-images.githubusercontent.com/101247575/225342862-1fda5d77-2bb4-4d09-80f6-eae40385c78b.png)
![image](https://user-images.githubusercontent.com/101247575/225343137-2e02ea98-8c7e-4884-b23a-47de4d588579.png)

Bản vẽ nhìn từ bên trong

![image](https://user-images.githubusercontent.com/101247575/225343223-810c34ca-b947-476b-ac35-af65e06fdb19.png)
![image](https://user-images.githubusercontent.com/101247575/225343236-efb47ac2-78ef-4dfc-b944-a4decea967b0.png)


Màu sắc

![image](https://user-images.githubusercontent.com/101247575/225343302-36ec602a-d5c4-4d8d-91f3-8e2f82f45dcf.png)
![image](https://user-images.githubusercontent.com/101247575/225343323-0842ffa3-82e6-4c72-95cd-c82311abc0a1.png)
![image](https://user-images.githubusercontent.com/101247575/225343329-0b0e51e6-c542-4d91-a405-c9a395d7da78.png)


Giao diện website
HOME
- Chứa hình ảnh sản phẩm, video quảng cáo cùng group Home
- Group Home chứa logo sản phẩm, username, ngày tháng năm
- Group Home chứa nhiệt độ, độ ẩm thành phố ta ở và số lượng rác trong thùng


![image](https://user-images.githubusercontent.com/101247575/225344431-90ff547a-116a-42ce-bf54-9d3ba64fbaec.png)
![image](https://user-images.githubusercontent.com/101247575/225343459-0514f8c5-749d-4594-88ea-31af40547659.png)

SETTINGS
- Ta có thể bật/tắt thông báo của thùng. Nếu tắt thì khi rác đầy hoặc thùng quá tải sẽ không được nghe audio cảnh báo nữa
- Ta có thể thay đổi màu của các nút
- Ta có thể cập nhật thông tin của chủ thùng rồi sau đó nhấn Save. 

![image](https://user-images.githubusercontent.com/101247575/225344465-64e8d480-3ad4-430e-8161-a6aab5ebe0c3.png)
![image](https://user-images.githubusercontent.com/101247575/225343692-c7c19538-0905-49bc-9464-a63fd205f6e0.png)

USER
- Chứa thông tin cá nhân mà người dùng mới nhập và thông tin thùng rác
- Ta có thể tải thông tin thùng rác về file txt

![image](https://user-images.githubusercontent.com/101247575/225343807-8b06fc99-c333-4c78-ba8f-3fd45a8d9eb8.png)
![image](https://user-images.githubusercontent.com/101247575/225343832-c28314ef-a45b-41b3-9b65-d3169ed20e6b.png)

FAN
- Ta có 2 cách để gửi nhiệt độ: dùng trực tiếp slider trên web hoặc dùng MQTT Explorer để gửi thông tin
- Khi nhiệt độ từ 50oC trở lên, cánh quạt thứ nhất sẽ bật để giảm nóng cho thùng
- Khi nhiệt độ từ 80oC trở lên, hai cánh quạt cùng bật và cảnh báo thùng quá tải sẽ xuất hiện

![image](https://user-images.githubusercontent.com/101247575/225343938-05bce1a6-1fef-4823-8306-70ea168a6a71.png)
![image](https://user-images.githubusercontent.com/101247575/225343960-729aa2e5-cc14-4d42-8c7f-f940e6d23b6a.png)

HISTORY
- Chứa những cảnh báo mà sản phẩm gửi về

![image](https://user-images.githubusercontent.com/101247575/225343995-2d5e468f-ce88-42ab-8613-df9bfd761889.png)
![image](https://user-images.githubusercontent.com/101247575/225344021-233d3ca8-7bbc-4f5d-bba4-8cd24317cf89.png)

TAB DATA
- Có 2 cách để gửi số lượng rác: dùng slider hoặc dùng MQTT Explorer gửi lên
- Sau khi có số lượng rác thì ta bấm nút INSERT để gửi số lượng rác
- Ta bấm REFRESH để cập nhật lại biểu đồ chỉ số lượng rác
- Cảnh báo rác đầy khi số lượng rác từ 80 trở lên 
- Sau khi đổ rác thì ta bấm CLEAR để số lượng rác trở về 0

![image](https://user-images.githubusercontent.com/101247575/225344371-05f46d44-d022-4a95-85ea-4ff097815487.png)


