# make_dataset_with_Naver_OCR

- 0 png2jpg.ipynb: 이미지 형식 변경 (선택사항)
- 1 naver_ocr_make_json.ipynb: naver_ocr 한 결과를 json 형식으로 저장
- 2 json_preprocessing.ipynb: 위 json파일에서 inferText와 coor정보만 저장
- 3 naver2labelme.ipynb: 위 json파일을 labelme.exe에서 실행할 수 있도록 형식 변경
- 4 make_dataset.ipynb: labelme를 통해 수정된 json파일을 참조하여 easyocr 학습이 가능한 dataset 생성 (이미지는 crop&resize 하여 따로 저장, label data는 csv파일로 저장)(easyocr은 csv파일에서 이미지 경로와 GT를 읽어옴)
