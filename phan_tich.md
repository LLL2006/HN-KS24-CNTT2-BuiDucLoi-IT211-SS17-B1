Nguyên nhân là do cấu hình hiện tại chỉ kiêểm tra đã đăng nhập hay chưa chuws k kiểm tra role để phaân quyền cho người duùng

Cấu hình hiện tại:

.authorizeHttpRequests(authorize -> authorize
.requestMatchers("/").permitAll()
.anyRequest().authenticated()
)

Ý nghĩa:

/ → ai cũng truy cập được.
anyRequest().authenticated() → mọi URL còn lại chỉ cần đăng nhập là được.