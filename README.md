# Dictionary App

Dictionary App은 RecyclerView를 사용하여 사용자에게 다양한 사전 항목을 보여주는 안드로이드 애플리케이션입니다. 각 항목은 제목과 설명을 포함하고 있으며, 항목을 클릭하면 자세한 내용을 보여주는 DetailActivity가 실행됩니다.

## 기능

- **RecyclerView**: 여러 사전 항목을 리스트 형식으로 표시
- **클릭 이벤트 처리**: 사용자가 리스트 항목을 클릭하면 해당 항목의 세부 정보를 볼 수 있는 DetailActivity 실행
- **비디오 및 이미지 표시**: 세부 정보 화면에서 관련 비디오와 이미지를 표시

## 파일 구조

- `app > manifests > AndroidManifest.xml`: 애플리케이션의 기본 구성 정보 및 각 액티비티에 대한 설정을 포함
- `java > com.example.dictionary.mRecyclerView`:
  - **ItemClickListener**: 리스트 항목 클릭 시 호출되는 인터페이스
  - **ListItem**: 리스트 항목의 데이터 모델 클래스 (제목, 설명, 비디오 파일, 이미지 파일 정보를 포함)
  - **MyAdapter**: RecyclerView의 어댑터로, 각 항목의 데이터를 뷰에 연결
  - **ViewHolder**: RecyclerView에서 각 항목의 뷰를 보유하는 클래스
- `java > com.example.dictionary`:
  - **DictionaryActivity**: RecyclerView를 사용하여 사전 항목 목록을 표시하는 메인 액티비티
  - **DetailActivity**: 리스트 항목을 클릭하면 항목의 세부 정보를 보여주는 액티비티 (비디오 및 이미지 포함)

- **딥러닝 수어 인식**: TensorFlow Lite를 사용하여 수어 이미지를 학습하고, 이를 바탕으로 실시간 수어 인식 기능 제공


