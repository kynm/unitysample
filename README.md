Tổng quan về unity 3D
I. Giới thiệu về Unity3D
Unity3D là phần mềm làm games trực tiếp theo thời gian thực, mà không cần render, cho phép người  design game có thể thiết kế InterfaceGraphic, map hay character … từ một phần mềm thứ 2 (thường là các phần mềm thiết kế đồ họa chuyên nghiệp như 3Dsmax, Blender, Maya, XSL,Cinema4D,Cheetah3D, Modo, Autodesk FBX, LightWave…) sau đó chỉ việc import nó vào trong Unity với định dạng của tập tin là *.FBX hay *.dae, *.3DS, *.dxf và *.obj, nhưng định dạng *.FBX hay được dùng vì được tối ưu hóa hơn, còn dùng các định dạng khác ngoài FBX thì phải cài phần mền thiết kế character tưng ứng thì mới dùng được (tức là dùng Maya có định dạng *.mb, *.ma thì muốn dùng được phải cài Maya)
Ngoài ra khi bạn design được một game thì bạn có thể xuất được ra một file.exe và có thể chạy và chơi được trên PC khác.
Một thế mạnh nữa của Unity là bạn có thể chạy demo game của bạn ngay trongkhi design, nó có hỗ trợ hai chế độ là Scene và Game, rất thuận tiện cho việc test thử các modulGame.
	Hỗ trợ cả unity 2D và unity 3D
Unity3D có 2 loại phiên bản, một cho người dùng free, và một phiên bản pro thì mất phí.
Khi tải Unity về các bạn cài đặt bình thường, đến khi kết thúc cài đặt nền các bạn chọn phiên bản Pro thì cần phải mua, còn nếu là người dùng free thì các bạn chọn kích  hoạt qua web, chỉ cần có kết nối mạng internet, sau đó chọn cài đặt thủ công và nhập mail, chọn free là bạn có thể sử dụng một bản Unity free.
II download và cài đạt
Để cài đặt unity phiên bản mới nhất có thể vào trang chủ tại 
http://unity3d.com/unity/download
lựa chọn phiên bản phù hợp với hệ điều hành mac hoặc window sau đó cài đặt bình thường


III, một số khái niệm cơ bản trong unity
1  Asset
Đây là kho tài nguyên cho việc xây dựng game trong một project của Unity. Các tài nguyên này có thể là hình ảnh, âm thanh, hoặc một mô hình 3D có sẵn. Unity sẽ tham chiếu đến các tập tin chúng ta sẽ sử dụng để tạo ra các tài nguyên cho trò chơi. Đây là lý do tại sao trong bất kỳ thư mục chứa project sử dụng Unity thì tất cả các tập tin tài nguyên phải được lưu trữ trong một thư mục con tên là Assets. 
 
Hình 2.2  Asset trong Unity  
2   Scene
Trong Unity, chúng ta có thể xem Scenes là các màn chơi, cấp độ chơi riêng lẻ, hoặc các vùng của nội dung trò chơi. Ví dụ như Main menu, Options, About …
Bằng cách xây dựng trò chơi với nhiều cảnh, chúng ta sẽ có thể phân phối thời gian tải và thử nghiệm các phần khác nhau của trò chơi riêng lẻ một cách nhanh chóng và chính xác.
 
Hình 2.3  Các scene của Unity 
3 Game Object
Khi một tài nguyên được sử dụng trong một scene, khi đó chúng ta có thể coi tài nguyên này là một “Game Object” mới. Mỗi GameObject phải chứa ít nhất một thành phần, đó là thành phần “Transform”. Transform chứa các phép để biến đổi góc quay, tỷ lệ hay tịnh tiến của đối tượng. Từ đây trong báo cáo này chúng em sẽ gọi GameObject trong cửa sổ Hierarchy là đối tượng game.
 
Hình 2.4  Kéo tài nguyên vào Scene để sử dụng
4 Component
Component là các thành phần trong một Game Object của Unity. Bằng cách đính kèm các thành phần vào cho một đối tượng, chúng ta có thể áp dụng ngay các phần mới của game engine vào đối tượng. Thông thường các thành phần này được Unity xây dựng sẵn như ánh sáng, camera, particle, hiệu ứng vật lý…
 
Hình 2.5  Các thành phần trong đối tượng Camera
5 Script
Script là thành phần quan trọng nhất trong Unity, có thể xem scripts như là linh hồn của game. Chúng ta có thể viết kịch bản cho game bằng C#, Java Scripts, hoặc Boo (một dẫn xuất của ngôn ngữ Python). Theo nhiều người đã sử dụng Unity thì code bằng C# sẽ giúp game chạy nhanh hơn và giúp kiểm soát code tốt hơn do tất cả các biến phải được khai báo rõ ràng. Mặt khác ngôn ngữ C# rất tiện dụng để lập trình, nên trong luận văn này, chúng em dùng ngôn ngữ C# để viết kịch bản cho game. Mỗi file script C# là một class bắt buộc kế thừa từ lớp MonoBehaviour, có tên class phải trùng với tên file script.
 
Hình 2.6  Cách tạo file script mới 
Giao diện code C# rất quen thuộc khi edit trên Visual Studio 2005
 
Hình 2.7  Lập trình Unity bằng C# trên Visual Studio 
Một đoạn script muốn thực thi được thì nó phải được gắn vào một đối tượng
 
Hình 2.8  Một file script đang gắn vào đối tượng 
6	Prefab
Hãy tưởng tượng Prefab là một cái thùng rỗng, mà bên trong nó chúng ta có thể chứa đựng các thành phần hay đối tượng khác nhau, chúng ta có thể viết kịch bản cho hành động của Prefab (khởi tạo, di chuyển, hay hủy đối tượng). Chúng ta có thể sử dụng đối tượng này nhiều lần trong trò chơi, và cũng có thể sử dụng lại cho project khác. Prefab cho phép chúng ta lưu trữ các đối tượng, toàn bộ thành phần bên trong và cấu hình hiện tại.
7  Material và Shader
Shader là đoạn script qui định cách thức render của chất liệu trên bề mặt vật thể. Material sử dụng shader để làm chất liệu cho mô hình. Giữa materials và shaders có mối liên hệ với nhau. Shaders qui định các thuộc tính cần để shader làm việc. Còn material cho phép gán hình ảnh vào các thuộc tính đó từ Asset.
 
Hình 2.9  Material và Shader 
IV , làm quen với giao diện quản lý của unity 3d
1 Cửa sổ Scene và Hierarchy
Cửa sổ Scene là nơi chúng ta sẽ xây dựng toàn bộ các đối tượng trong game. Cửa sổ cung cấp nhiều góc nhìn khác nhau, có thể nhìn dạng phối cảnh hoặc dạng song song. Chúng ta có thể kéo thả đối tượng trên cửa sổ này, di chuyển, xoay…
 
Cửa sổ Scene cũng kèm theo bốn nút điều khiển tiện lợi như hình trên. Truy cập từ bàn phím bằng cách sử dụng các phím Q, W, E, và R. Các phím thực hiện các hoạt động sau đây:
o	Công cụ bàn tay [Q]: công cụ này cho phép di chuyển trong cửa sổ Scene, xoay góc nhìn, phóng to, thu nhỏ góc nhìn.
o	Công cụ di chuyển [W]: Công cụ này dùng để di chuyển một đối tượng.
o	Công cụ xoay [E]: Công cụ này cho phép chúng ta xoay nhân vật theo một trục nào đó trong không gian.
o	Công cụ tỷ lệ [R]: Công cụ này cho phép chúng ta tăng giảm tỷ lệ kích thước của đối tượng.
Khi chọn một đối tượng trong cửa sổ Scene, đối tượng này sẽ được tự động chọn trong cửa sổ Hierarchy và ngược lại.

2	 Inspector
Inspector sẽ hiển thị tất cả thông tin, các thành phần trong đối tượng game đang chọn, và cho phép điều chỉnh các biến của các thành phần này. Có thể xem cửa sổ này như cửa sổ Properties khi design giao diện Winform trên Visual Studio
3	 Cửa sổ Game
Cửa sổ này sẽ hiển thị những gì có trong cửa sổ Scene và sẽ hoạt động khi nhấn nút Play. Trong cửa sổ này chúng ta có thể chọn các kích cỡ hiển thị khác nhau để build cho các loại máy khác nhau. Chúng ta có thể chơi thử game trên cửa sổ này khi đã nhấn nút Play. Lưu ý rằng khi cửa sổ này hoạt động rồi thì mọi chỉnh sửa trên cửa sổ Scene và cài đặt cho các đối tượng chỉ là tạm thời và khi nhấn nút Stop, cửa sổ này về lại trạng thái tĩnh thì mọi chỉnh sửa trước đó là không còn.
4  Cửa sổ Project
Cửa sổ Project thể hiện nội dung bên trong thư mục Assets của project chúng ta. Khi thêm tài nguyên vào thư mục Assets ngay lập tức chúng sẽ tự động được cập nhập vào project Unity của chúng ta.



V. sample project
Name: clone code flappy bird
Mục đích: làm quen và hiểu các bước làm game unity 2d
Hướng dẫn: học và làm theo tutorial 
http://vietgamedev.net/blog/1212/unity-tut-h%C6%B0%E1%BB%9Bng-d%E1%BA%ABn-l%C3%A0m-game-flappy-bird-b%E1%BA%B1ng-unity/
http://vietgamedev.net/blog/1213/unity-tut-h%C6%B0%E1%BB%9Bng-d%E1%BA%ABn-l%C3%A0m-game-flappy-bird-b%E1%BA%B1ng-unity-k%C3%AC-2/
http://vietgamedev.net/blog/1228/unity-tut-h%C6%B0%E1%BB%9Bng-d%E1%BA%ABn-l%C3%A0m-game-flappy-bird-b%E1%BA%B1ng-unity-k%C3%AC-3/

lý do: tutorial khá đơn giản giới thiệu chi tiết cho người mới bắt đầu. ngoài ra đây là game khá nổi tiếng và tạo hứng thú cho người code :D
resource:  https://github.com/kynm/unitysample

