# 프로젝트 제목 : tagme
>NFC 태그를 활용한 음식점 주문/결제 자동화 어플리케이션
## 1.결과물
<div>
    <img src="https://user-images.githubusercontent.com/43267195/83626990-3f7b1400-a5d1-11ea-8a3e-c5571482291d.png">
</div>

## 2. 환경설정
- Build.gradle(module)
```
// ted permission
    implementation 'gun0912.ted:tedpermission:2.1.1'
    // Gson
    implementation 'com.google.code.gson:gson:2.8.5'
    // retrofit
    implementation 'com.squareup.retrofit2:retrofit:2.4.0'
    implementation 'com.squareup.retrofit2:converter-gson:2.4.0'
    implementation 'com.jakewharton.retrofit:retrofit2-rxjava2-adapter:1.0.0'
    // rxJava
    implementation 'io.reactivex.rxjava2:rxandroid:2.1.0'
    implementation 'io.reactivex.rxjava2:rxjava:2.2.0'
    // okhttp
    implementation 'com.squareup.okhttp3:okhttp:3.10.0'
    implementation 'com.squareup.okhttp3:logging-interceptor:3.9.1'
    // naver map api
    implementation 'com.naver.maps.open:naver-map-api:2.1.2@aar'
    // firebase dynamic link
    implementation 'com.google.firebase:firebase-core:16.0.4'
    implementation 'com.google.firebase:firebase-dynamic-links:16.1.2'
    // glide
    implementation 'com.github.bumptech.glide:okhttp3-integration:4.8.0'
    annotationProcessor 'com.github.bumptech.glide:compiler:4.8.0'
```
- Manifest
```
<uses-feature
        android:name="android.hardware.nfc"
        android:required="false" />

    <!-- NFC 퍼미션 -->
    <uses-permission android:name="android.permission.NFC" />
    <!-- HTTP 퍼미션 -->
    <uses-permission android:name="android.permission.INTERNET" />
    <!-- GPS 퍼미션 -->
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
    <!-- 와이파이 퍼미션-->
    <uses-permission android:name="android.permission.ACCESS_WIFI_STATE" />
    <uses-permission android:name="android.permission.CHANGE_WIFI_STATE" />
```
