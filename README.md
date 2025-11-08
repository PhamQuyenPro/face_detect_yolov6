# face_detect_yolov6
Dự án dùng yolov6 đề phát hiện khuôn mặt trong hình ảnh và video

# Cài đặt môi trường chạy  
Sử dụng docker: 
Bước 1: docker pull quyenpd/quyenpd:v1.1
Bước 2: docker run -dit --ipc=host -v $(pwd):/face_detect_yolov6 --name quyenpd quyenpd/quyenpd:v1.1
Bước 3: docker exec -it quyenpd /bin/bash

# Cách chạy (trong container docker)
python tools/infer.py --weights weights/yolov6s-face.pt --source data/images/
