
# First Move Demo

## Giới thiệu

`first-move-demo` là một dự án demo đơn giản sử dụng ngôn ngữ Move trên nền tảng Aptos. Dự án này triển khai một hợp đồng thông minh (smart contract) cơ bản với chức năng "Hello, World!" nhằm giúp bạn làm quen với Move và hệ sinh thái Aptos.

## Yêu cầu

Trước khi bắt đầu, hãy đảm bảo bạn đã cài đặt các công cụ sau:

-   Aptos CLI
    
-   Move Compiler
    
-   Git
    
-   Một tài khoản Aptos (có thể tạo bằng Aptos CLI)
    

## Cài đặt

1.  Clone repository:
    
    ```
    git clone https://github.com/yourusername/first-move-demo.git
    cd first-move-demo
    ```
    
2.  Cấu hình Aptos:
    
    ```
    aptos init
    ```
    
    Làm theo hướng dẫn để thiết lập tài khoản và chuỗi khối.
    

## Triển khai hợp đồng Move

1.  Biên dịch hợp đồng:
    
    ```
    aptos move compile --package-path .
    ```
    
2.  Đăng ký hợp đồng lên mạng Aptos:
    
    ```
    aptos move publish --package-path . --profile default
    ```
    

## Chạy hợp đồng

Sau khi triển khai hợp đồng, bạn có thể gọi hàm `hello_world` bằng lệnh:

```
aptos move run --function-id 'default::helloworld::hello' --profile default
```

Hàm này sẽ trả về chuỗi `"Hello, World!"`.

## Cấu trúc thư mục

```
first-move-demo/
│── sources/
│   └── helloworld.move  # Hợp đồng Move chính
│── Move.toml            # Cấu hình Move package
│── README.md            # Tài liệu hướng dẫn
```

## Góp ý

Nếu bạn có bất kỳ câu hỏi hoặc ý tưởng nào để cải thiện dự án, hãy tạo issue hoặc pull request trên GitHub!

## Bản quyền

Dự án này được phát hành theo giấy phép MIT.
