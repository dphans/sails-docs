# app.js

### Ý Tưởng

File khởi chạy ứng dụng SailsJs trong NodeJS, code trong file này chỉ được thực thi khi ứng dụng ở trạng thái `production`.

Khi bạn deploy ứng dụng của mình trong máy tính cá nhân, sử dụng cú pháp `sails lift`, code trong file `app.js` sẽ không được thực thi. Bằng cách khác, nếu như bạn muốn khởi chạy server mà không muốn dụng `sails lift`, bạn vẫn có thể khởi chạy file này theo cách thông thường như `node app` hay `npm start`,... Theo cách này, ứng dụng sẽ ở trạng thái `production`.

Ví dụ, nếu bạn sử dụng các dịch vụ PaaS như [Heroku](http://heroku.com), server sẽ tự động phát hiện bạn đang deploy một ứng dụng NodeJS. Khi thực thi, server tự động gán thêm biến môi trường (`NODE_ENV`) vào và đặt ứng dụng ở trạng thái `production`.

> Trong lúc deploy (`development`) đến release một ứng dụng (`production`), có thể bỏ qua file `app.js`. Nếu như bạn muốn tìm hiểu thêm, hay muốn sử dụng Sails một cách thủ công, viết automated tests, migrate database một cách thủ công,... bạn có thể xem qua `app.js`.

<docmeta name="displayName" value="app.js">
